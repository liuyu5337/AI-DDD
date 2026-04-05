---
name: openapi-first-contract
description: Execution checklist for designing or aligning OpenAPI-first contracts
disable-model-invocation: true
user-invocable: false
---

# OpenAPI Contract Checklist / OpenAPI 合同检查清单

Source of truth / 规则来源:
- `.claude/rules/api-contract-rules.md`
- `.claude/rules/response-error-rules.md`

## When using this skill / 使用方式
Before coding or reviewing an API change, check:
1. What is the endpoint purpose?
2. What are the request and response DTOs?
3. What validation rules apply?
4. How are pagination, filter, and sort represented?
5. What error codes and error envelope are returned?
6. What compatibility or migration note is needed?
7. What frontend assumption must be stated explicitly?
