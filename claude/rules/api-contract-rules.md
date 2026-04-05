# API Contract Rules / API 合同规则

## OpenAPI first
For new or changed APIs, define first:
- endpoint purpose
- request model
- response model
- validation rules
- error model
- pagination/filter/sort conventions
- idempotency requirement where relevant
- compatibility notes

## Contract boundaries
- Do not expose DO, MyBatis-Plus models, wrappers, or page objects directly.
- Do not let table structure dictate API shape directly.
- Make frontend-backend integration assumptions explicit.
- Do not leave field meaning ambiguous.

## Compatibility
- Prefer stable DTOs.
- Breaking changes must be called out explicitly.
- Default to additive evolution when possible.
