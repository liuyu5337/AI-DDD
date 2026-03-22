---
name: db-sql-migration
description: SQL-script-based schema/data change and rollback rules
disable-model-invocation: true
user-invocable: false
---
# SQL Migration Rules

When database changes are needed, always describe:
- schema changes
- data changes
- execution order
- rollback or mitigation strategy
- index impact
- compatibility impact

Rules:
- Deliver changes as SQL scripts.
- Avoid destructive operations without explicit warning.
- Design indexes from real query patterns.
- Consider nullability, defaults, uniqueness, and large-table impact.
- Call out high-risk DDL/DML clearly.