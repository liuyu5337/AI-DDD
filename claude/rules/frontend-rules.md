# Frontend Rules / 前端规则

## Baseline
- Vue 3
- Composition API
- Element Plus

## UI and state
- Pages compose behavior; do not bury heavy business logic in templates.
- Loading, empty, error, and permission states must be explicit.
- Destructive actions require confirmation.
- Repeated patterns should be extracted into reusable components or composables.

## API integration
- API calls must be centralized in dedicated modules.
- Do not scatter request code across page components.
- Request/response typing and naming must stay consistent with agreed contracts.
- Do not silently change backend assumptions in UI code.
