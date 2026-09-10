---
name: Create and cancel a dispatch work order
description: Create a dispatch work order against a project, attach activities, and
  cancel it safely, respecting the parts of the Aerones write surface that have no
  replay protection.
api: openapi/aerones-operations-hub-openapi.json
operations:
- core_endpoints_projects_list_projects
- core_endpoints_projects_get_project
- core_endpoints_robot_sets_list_robot_sets
- dispatch_api_workorders_list_workorders
- dispatch_api_workorders_create_workorder
- dispatch_api_workorders_get_workorder
- dispatch_api_workorders_create_workorder_activity
- dispatch_api_workorders_cancel_workorder
- dispatch_api_workorders_delete_workorder
---

# Create and cancel a dispatch work order

This skill writes. Read the safety rules before the steps.

## Safety rules for this API

- **There is no `Idempotency-Key` header anywhere in this contract.**
  `dispatch_api_workorders_create_workorder` is **not** idempotent. If a POST times out,
  do **not** blind-retry — call `dispatch_api_workorders_list_workorders` and check
  whether the work order landed. A retry creates a second one.
- **Cancel is reversible-ish, delete is not.** `dispatch_api_workorders_cancel_workorder`
  (`POST /api/dispatch/v1/workorders/{workorder_id}/cancel`) is the safe way to undo a
  creation. `dispatch_api_workorders_delete_workorder`
  (`DELETE /api/dispatch/v1/workorders/{workorder_id}`) is not, and no restore path for
  a work order exists in this contract. Prefer cancel.
- **No dry run.** There is no preview or simulate flag. Every write is real.
- **No stated reversal window.** Aerones publishes no documentation giving a time limit
  on cancellation. What the contract does say, for the sibling team-request and
  set-request cancels, is that any non-terminal state moves to `CANCELLED` — reversal is
  bounded by lifecycle state, not by a clock. Do not tell a user they have "N days".

## Steps

1. **Locate the project.** `core_endpoints_projects_list_projects`
   (`GET /api/core/v1/projects`) or `core_endpoints_projects_search_projects`
   (`GET /api/core/v1/projects/search`), then `core_endpoints_projects_get_project`
   (`GET /api/core/v1/projects/{project_id}`) to confirm you have the right one.
2. **Check the resource.** `core_endpoints_robot_sets_list_robot_sets`
   (`GET /api/core/v1/robot-sets`) — a work order is executed by a robot set.
3. **Check for an existing work order first.**
   `dispatch_api_workorders_list_workorders` (`GET /api/dispatch/v1/workorders`). This
   step is the replacement for the idempotency the API does not have.
4. **Create.** `dispatch_api_workorders_create_workorder`
   (`POST /api/dispatch/v1/workorders`). Record the returned id immediately.
5. **Verify.** `dispatch_api_workorders_get_workorder`
   (`GET /api/dispatch/v1/workorders/{workorder_id}`).
6. **Add activities.** `dispatch_api_workorders_create_workorder_activity`
   (`POST /api/dispatch/v1/workorder-activities`). Same non-idempotency warning applies.
   For many at once, `dispatch_api_workorders_bulk_create_workorders`
   (`POST /api/dispatch/v1/workorders/bulk`) exists — one call is safer than a loop of
   non-idempotent calls.
7. **Undo, if needed.** `dispatch_api_workorders_cancel_workorder`.

## Error handling

The declared error body is `{code, message}` with `code` in
`validation | server | auth | unknown | external | generic`. `400` is the only failure
status declared on most write operations. An `external` code means a downstream system
(NetSuite, Wrike, Pipedrive) failed, not your request — that is the one class worth
retrying, and only after checking step 3.
