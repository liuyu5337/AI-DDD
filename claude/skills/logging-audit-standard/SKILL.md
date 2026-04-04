---
name: logging-audit-standard
description: Logging and audit rules for backend and sensitive operations
disable-model-invocation: true
user-invocable: false
---
# Logging and Audit Standard / 日志与审计规范

## Logging / 日志
- Log with useful business context / 带业务上下文记录日志
- Include requestId/traceId when possible
- Record key identifiers such as orderNo, customerId, billNo where relevant
- Avoid noisy logs with no diagnostic value / 避免无诊断价值的噪声日志
- Never log secrets, passwords, tokens, or sensitive personal data

## Audit / 审计
Sensitive operations should be auditable / 敏感操作应具备审计能力:
- create/update/delete
- approval/reject
- import/export
- authorization changes
- login/security-sensitive actions

Audit records should include / 审计记录建议包含:
- operator
- operation time
- module
- target object
- action type
- result
- failure reason if any
- requestId if available
