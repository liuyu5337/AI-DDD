---
name: response-error-standard
description: Unified response, error-code, and exception-handling rules for this project
disable-model-invocation: true
user-invocable: false
---
# Response and Error Standard

## Unified Response Rules
- Use a stable response envelope for normal JSON APIs.
- Recommended fields: code, message, data, requestId.
- Do not expose stack traces, SQL text, or framework internals to clients.
- Separate business failure from system failure clearly.

## Pagination Rules
- Convert pagination results to project-defined DTOs.
- Do not expose MyBatis-Plus Page objects directly.
- Recommended fields: records, total, pageNo, pageSize.

## Error Code Rules
- Use stable, semantic string-based error codes.
- Keep shared error codes separate from module-specific error codes.
- Do not hardcode random error code strings in controllers.

## Exception Handling Rules
- Use global exception handling.
- Handle business exceptions, validation exceptions, permission exceptions, and unknown exceptions separately.
- Include requestId or trace information in error responses where appropriate.