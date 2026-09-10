---
name: Look up a customer's turbines and their blade anomalies
description: Resolve a customer to their turbines, then pull the anomaly findings and
  attached inspection media for a blade, using the Aerones Operations Hub REST API.
api: openapi/aerones-operations-hub-openapi.json
operations:
- list_customers
- list_customer_turbines
- get_customer_turbine
- list_turbine_models
- list_anomaly_types
- list_anomalyrecommendations
- core_endpoints_anomalies_files_get_anomaly_files
---

# Look up a customer's turbines and their blade anomalies

Read-only. Every operation here is a `GET`, so nothing in this skill can change state.

## Before you start

- Base URL is `https://operations.aerones.com`. Every path in the contract already
  carries the `/api` prefix.
- Send `Authorization: Bearer <token>`. Tokens come from the Keycloak realm at
  `https://sso.aerones.com/realms/aerones` (client `operations-hub`), **not** from
  Aerones' website. There is no public sign-up and no self-service API key: if you do
  not already have credentials, stop and ask the customer's Aerones contact.
- The OpenAPI description is served anonymously at `/api/openapi.json`. The data is not.

## Steps

1. **Find the customer.** `list_customers` — `GET /api/core/v1/customers`. Use the
   `search` query parameter rather than paging the whole list. Note that
   `customers_api_get_customers` (`GET /api/customers`) does the same thing and is
   **deprecated** — use the `/core/v1/` one.
2. **List their turbines.** `list_customer_turbines` —
   `GET /api/core/v1/customers/{customer_id}/turbines`. This is scoped to one customer;
   `list_turbines` (`GET /api/core/v1/turbines`) is the unscoped fleet view.
3. **Resolve the model.** A turbine references a turbine model; `list_turbine_models`
   (`GET /api/core/v1/turbine-models`) gives manufacturer, model and the blade geometry
   the anomaly coordinates are expressed against.
4. **Read the anomaly taxonomy first.** `list_anomaly_types`
   (`GET /api/core/v1/anomaly-types`) and `list_anomalyrecommendations`
   (`GET /api/core/v1/anomaly-recommendations`). Anomaly records reference these by id,
   so without them a finding is a set of integers.
5. **Pull the evidence.** `core_endpoints_anomalies_files_get_anomaly_files` —
   `GET /api/core/v1/anomalies/{id}/files/` returns the media attached to one anomaly.

## Conventions that apply

- **Pagination is opt-in.** Pass `paginate=true` with `page` and `page_size`. Without
  `paginate`, a list endpoint may return everything.
- **Filtering** is `search` (free text) and `sort`; there is no `expand`/`include`.
- **Errors** are `{ "code": "<validation|server|auth|unknown|external|generic>",
  "message": "..." }` — not RFC 9457. The contract declares only `400` and `404`, so
  treat an undeclared status as possible: a `401` or `5xx` will not match the schema.
- **Do not assume rate limits are absent.** None are documented and no `429` is
  declared, which means you get no `Retry-After` to back off against. Pace requests
  conservatively.

## What this skill deliberately does not do

Nothing here writes. If the task calls for creating an anomaly, an offer or a work
order, use a different skill and re-read `conventions/aerones-conventions.yml` first —
most of the write surface has **no** idempotency protection, so a retried request
creates a duplicate.
