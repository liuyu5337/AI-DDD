---
name: db-sql-migration
description: SQL-script based schema/data change rules for backend delivery
disable-model-invocation: true
user-invocable: false
---

# DB SQL Migration / 数据库变更规范

## Core rules
- use reviewed SQL scripts for schema/data changes
- separate schema change and data fix scripts where practical
- explain rollback or mitigation
- avoid destructive changes without explicit warning

## Review focus
- naming
- indexes
- default values
- nullability
- constraints
- compatibility risk
