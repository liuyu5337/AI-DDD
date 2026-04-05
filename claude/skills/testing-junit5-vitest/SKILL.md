---
name: testing-junit5-vitest
description: Test design and reporting checklist aligned with repository-wide testing rules
disable-model-invocation: true
user-invocable: false
---

# Testing Checklist / 测试清单

Source of truth / 规则来源:
- `.claude/rules/testing-rules.md`

## Backend / 后端
- app service behavior
- domain rule coverage
- controller/integration tests when contract behavior matters

## Frontend / 前端
- rendering states
- user interactions
- validation and edge cases

## Report / 报告
- what was tested
- what passed / failed
- what remains untested
