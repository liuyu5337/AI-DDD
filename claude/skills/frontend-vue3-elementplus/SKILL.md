---
name: frontend-vue3-elementplus
description: Vue 3 + Element Plus frontend rules for this project
disable-model-invocation: true
user-invocable: false
---

# Frontend Rules / 前端规则

## Baseline / 基线
- Vue 3
- Composition API
- Element Plus

## Rules / 规则
- Keep views focused on composition / 页面负责组合，不承载复杂业务
- Avoid heavy business logic in templates / 模板避免重业务逻辑
- Centralize API calls / API 调用集中管理
- Prefer reusable components for repeated patterns / 重复模式优先抽组件
- Make loading, empty, and error states explicit / 明确各种状态
- Keep labels, placeholders, and messages consistent / 标签、占位符、提示语保持一致
- Use clear form validation and confirmation for destructive actions / 高风险操作需确认
