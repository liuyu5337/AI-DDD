---
name: testing-junit5-vitest
description: Testing rules using JUnit 5 for backend and Vitest + Vue Test Utils for frontend
disable-model-invocation: true
user-invocable: false
---

# Testing Rules / 测试规则

## General / 通用
- Add or update tests for meaningful behavior changes / 有意义行为变化要补测试
- Prefer targeted, maintainable tests / 优先针对性且可维护的测试
- Cover success paths, validation failures, and important edge cases / 覆盖成功路径、校验失败、重要边界

## Backend / 后端
- Use JUnit 5
- Prioritize application-service behavior and domain rules / 优先测应用服务与领域规则
- Add controller/integration tests when contract behavior is important / 合同行为重要时补控制器/集成测试

## Frontend / 前端
- Use Vitest + Vue Test Utils
- Cover rendering states, interactions, validation, and critical component behavior / 覆盖渲染状态、交互、校验、关键组件行为

## Delivery Rule / 交付规则
Completion reports must include / 完成时必须说明:
- what was tested
- what passed or failed
- what remains untested
