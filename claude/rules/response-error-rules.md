# Response and Error Rules / 响应与错误规则

## Unified response
- Use a stable response envelope.
- Recommended fields: `code`, `message`, `data`, `requestId`.
- Do not expose stack trace, SQL text, or framework internals to clients.
- Separate business failure from system failure clearly.

## Pagination
- Convert paging results into project-defined DTOs.
- Do not expose MyBatis-Plus page objects directly.
- Recommended fields: `records`, `total`, `pageNo`, `pageSize`.

## Error handling
- Use global exception handling.
- Distinguish validation, business, permission, integration, and unknown failures.
- Error codes should be stable and semantic.
