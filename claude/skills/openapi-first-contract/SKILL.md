---
name: openapi-first-contract
description: OpenAPI-first API design rules for frontend-backend separated systems
disable-model-invocation: true
user-invocable: false
---
# OpenAPI First Rules

For new or changed APIs, define first:
- endpoint purpose
- request model
- response model
- validation rules
- error codes / error structure
- pagination/filter/sort rules
- idempotency requirements where relevant
- compatibility strategy

Rules:
- Prefer stable contracts.
- Keep field naming consistent.
- Do not expose persistence DO or MyBatis-Plus models directly.
- Make integration assumptions explicit.
- Document breaking changes clearly.