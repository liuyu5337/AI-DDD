---
name: logging-audit-standard
description: Logging and audit implementation checklist aligned with repository-wide logging rules
disable-model-invocation: true
user-invocable: false
---

# Logging and Audit Checklist / 日志与审计清单

Source of truth / 规则来源:
- `.claude/rules/logging-audit-rules.md`

## Check / 检查
- key business context in logs
- requestId / traceId propagation
- no secrets in logs
- auditable records for sensitive actions
- failure reason recorded where useful
