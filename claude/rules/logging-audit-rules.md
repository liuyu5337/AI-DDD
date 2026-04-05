# Logging and Audit Rules / 日志与审计规则

## Logging
- Log with useful business context.
- Include requestId / traceId when possible.
- Prefer meaningful identifiers such as orderNo, billNo, customerId when relevant.
- Avoid noisy logs with no diagnostic value.
- Never log secrets or sensitive personal data.

## Audit
Sensitive operations should be auditable, including:
- create / update / delete
- approval / reject
- import / export
- permission changes
- login or security-sensitive actions

Audit records should capture where relevant:
- operator
- operation time
- module
- target object
- action type
- result
- failure reason
- requestId
