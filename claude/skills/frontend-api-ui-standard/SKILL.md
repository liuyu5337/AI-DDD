---
name: frontend-api-ui-standard
description: Frontend API-layer and UI consistency rules for Vue 3 + Element Plus

disable-model-invocation: true
user-invocable: false
---
# Frontend API and UI Standard

## API Layer Rules
- Centralize API requests in dedicated modules.
- Do not scatter request code across page components.
- Keep request/response typing consistent.
- Use shared error-handling patterns.

## UI Rules
- List pages should remain structurally consistent.
- Forms require validation and clear feedback.
- Destructive operations require confirmation.
- Loading, empty, and error states must be explicit.
- Reuse shared dialogs, tables, and form patterns when appropriate.