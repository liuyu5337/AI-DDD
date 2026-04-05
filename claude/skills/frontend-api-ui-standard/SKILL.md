---
name: frontend-api-ui-standard
description: Frontend API integration and UI consistency rules
disable-model-invocation: true
user-invocable: false
---

# Frontend API + UI Standard / 前端接口与界面规范

## API integration
- centralize request functions
- explicit request / response mapping
- loading / error / retry handling should be visible

## UI consistency
- same interaction pattern should use same component pattern
- destructive actions need confirmation
- permission-limited actions should have clear disabled/hidden behavior
