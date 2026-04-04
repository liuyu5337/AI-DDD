---
name: db-sql-migration
description: SQL-script-based schema/data change and rollback rules
disable-model-invocation: true
user-invocable: false
---
# SQL Migration Rules / SQL 迁移规则

When database changes are needed, always describe / 涉及数据库变更时始终说明:
- schema changes
- data changes
- execution order
- rollback or mitigation strategy
- index impact
- compatibility impact

Rules / 规则:
- Deliver changes as SQL scripts / 以 SQL 脚本交付
- Avoid destructive operations without explicit warning / 破坏性操作必须警示
- Design indexes from real query patterns / 索引设计基于真实查询模式
- Consider nullability, defaults, uniqueness, and large-table impact / 考虑空值、默认值、唯一性、大表影响
- Call out high-risk DDL/DML clearly / 明确高风险 DDL/DML
