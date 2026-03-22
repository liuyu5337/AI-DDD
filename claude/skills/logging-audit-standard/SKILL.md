---
name: logging-audit-standard
description: Logging and audit rules for backend and sensitive operations
disable-model-invocation: true
user-invocable: false
---
# Logging and Audit Standard

## Logging Rules
- Log with useful business context.
- Include requestId/traceId when possible.
- Record key identifiers such as orderNo, customerId, billNo where relevant.
- Avoid noisy logs with no diagnostic value.
- Never log secrets, passwords, tokens, or sensitive personal data.

## Audit Rules
Sensitive operations should be auditable, especially:
- create/update/delete
- approval/reject
- import/export
- authorization changes
- login/security-sensitive actions

Audit records should include:
- operator
- operation time
- module
- target object
- action type
- result
- failure reason if any
- requestId if available