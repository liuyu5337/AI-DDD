---
name: prepare-sql-change
description: Prepare SQL schema/data change plan and rollback notes
disable-model-invocation: true
context: fork
agent: db-helper
---
Prepare SQL change guidance for:

$ARGUMENTS

Required output:
- schema/data impact
- SQL change plan
- execution order
- rollback or mitigation
- risks
- index suggestions