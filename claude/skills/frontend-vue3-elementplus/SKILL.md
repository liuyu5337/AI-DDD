---
name: frontend-vue3-elementplus
description: Vue 3 + Element Plus implementation method aligned with repository-wide frontend rules
disable-model-invocation: true
user-invocable: false
---

# Frontend Execution Method / 前端实现方法

Source of truth / 规则来源:
- `.claude/rules/frontend-rules.md`
- `.claude/rules/api-contract-rules.md`

## Implementation pattern / 实现套路
1. Clarify page goal and primary user actions.
2. Split page composition, business state, and API integration cleanly.
3. Centralize API requests.
4. Make loading / empty / error / permission states explicit.
5. Extract repeated patterns into reusable components or composables.
6. Add or update Vitest tests for critical behavior.
