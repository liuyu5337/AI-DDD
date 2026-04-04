---
name: openapi-first-contract
description: OpenAPI-first API design rules for frontend-backend separated systems
disable-model-invocation: true
user-invocable: false
---
# OpenAPI First Rules / OpenAPI 先行规则

For new or changed APIs, define first / 新增或修改接口时先定义:
- endpoint purpose
- request model
- response model
- validation rules
- error codes / error structure
- pagination/filter/sort rules
- idempotency requirements where relevant
- compatibility strategy

Rules / 规则:
- Prefer stable contracts / 优先稳定合同
- Keep field naming consistent / 字段命名一致
- Do not expose persistence DO or MyBatis-Plus models directly
- Make integration assumptions explicit / 明确集成假设
- Document breaking changes clearly / 明确记录破坏性变更
