---
name: sql-script-naming-standard
description: SQL script naming checklist aligned with database and naming rules
disable-model-invocation: true
user-invocable: false
---

# SQL Naming Checklist / SQL 命名清单

Source of truth / 规则来源:
- `.claude/rules/database-rules.md`
- `.claude/rules/naming-rules.md`

Recommended naming pattern:
- `YYYYMMDDHHmm__module__change_intent.sql`

Checklist:
- sortable by time
- module visible
- intent visible
- not vague like `fix.sql` or `update.sql`
