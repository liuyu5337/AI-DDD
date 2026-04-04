---
name: prepare-sql-change
description: Prepare SQL schema/data change plan and rollback notes
disable-model-invocation: true
context: fork
agent: db-helper
---
Prepare SQL change guidance for / 为以下变更准备 SQL 方案:

$ARGUMENTS

Required output:
- schema/data impact
- SQL change plan
- execution order
- rollback or mitigation
- risks
- index suggestions
