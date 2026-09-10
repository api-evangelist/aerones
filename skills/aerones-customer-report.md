---
name: Request and collect a customer report
description: Request a custom Aerones report over a selection of turbines or locations,
  poll it to completion, and download it — the customer-portal flow.
api: openapi/aerones-operations-hub-openapi.json
operations:
- customer_portal_custom_report_types
- customer_portal_start_custom_report
- customer_portal_list_custom_reports
- customer_portal_custom_report_status
- customer_portal_download_custom_report
- customer_portal_download_daily_report
- customer_portal_download_final_report
---

# Request and collect a customer report

This is the asynchronous report flow behind `portal.aerones.com`. It is the closest
thing in the contract to a customer-facing capability rather than an internal one.

## Steps

1. **Ask what can be reported on.** `customer_portal_custom_report_types` —
   `GET /api/core/v1/reports/custom/types`. Do not hard-code a report type; the list is
   server-side and unversioned.
2. **Submit the request.** `customer_portal_start_custom_report` —
   `POST /api/core/v1/reports/custom`, over a selection of turbines or locations. This
   returns a `generation_id`.
   **This POST is not idempotent.** If it times out, call
   `customer_portal_list_custom_reports` (`GET /api/core/v1/reports/custom`) and look for
   your request before submitting again.
3. **Poll.** `customer_portal_custom_report_status` —
   `GET /api/core/v1/reports/custom/{generation_id}/status`. There is no webhook and no
   callback: polling is the only completion signal this API offers. No `Retry-After` is
   returned, so choose your own interval and back off — a few seconds, widening.
4. **Download.** `customer_portal_download_custom_report` —
   `GET /api/core/v1/reports/custom/{generation_id}/download`.

## The other two report shapes

- `customer_portal_download_daily_report` — `POST /api/core/v1/reports/daily` renders and
  returns a daily report PDF synchronously.
- `customer_portal_download_final_report` — `POST /api/core/v1/reports/final` returns the
  final service-order-line report, either engine-rendered or the uploaded file.
- Do **not** use `customer_portal_download_final_report_file`
  (`GET /api/core/v1/reports/final/{service_order_line_id}/file`) in new work: it is
  flagged **deprecated** in the contract. No sunset date is published, so treat it as
  liable to disappear without notice.

## Conventions

- Auth: `Authorization: Bearer <token>` from `https://sso.aerones.com/realms/aerones`,
  or the `opshub_prod_sessionid` session cookie in a browser context.
- Errors: `{code, message}`; only `400` and `404` are declared. A polling loop should
  treat any undeclared status as terminal-unknown rather than retrying forever.
- Terms of service acceptance is itself an operation on this surface
  (`list_terms_of_services`, `create_user_tos_acceptance`) — a portal user may need to
  accept before reports resolve.
