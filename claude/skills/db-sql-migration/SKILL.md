---
name: db-sql-migration
description: SQL-script-based schema/data change execution checklist
disable-model-invocation: true
user-invocable: false
---

# SQL Change Checklist / SQL 变更清单

Source of truth / 规则来源:
- `.claude/rules/database-rules.md`

## Always describe / 必须说明
- schema changes
- data changes
- execution order
- rollback or mitigation
- index impact
- compatibility impact

## Review points / 审核点
- nullability
- default values
- uniqueness
- large-table impact
- high-risk DDL or DML
