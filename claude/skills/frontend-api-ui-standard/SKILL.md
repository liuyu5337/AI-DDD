---
name: frontend-api-ui-standard
description: Frontend API-layer and UI consistency rules for Vue 3 + Element Plus
disable-model-invocation: true
user-invocable: false
---
# Frontend API and UI Standard / 前端 API 与 UI 规范

## API Layer / API 层
- Centralize API requests in dedicated modules / API 请求集中在专门模块
- Do not scatter request code across page components / 不要把请求逻辑散在页面组件
- Keep request/response typing consistent / 保持请求响应类型一致
- Use shared error-handling patterns / 统一错误处理模式

## UI Rules / UI 规则
- List pages should remain structurally consistent / 列表页结构统一
- Forms require validation and clear feedback / 表单需校验并有清晰反馈
- Destructive operations require confirmation / 高风险操作需要确认
- Loading, empty, and error states must be explicit
- Reuse shared dialogs, tables, and form patterns when appropriate / 优先复用共享模式
