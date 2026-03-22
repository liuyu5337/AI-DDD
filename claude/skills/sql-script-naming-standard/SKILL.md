---
name: sql-script-naming-standard
description: SQL script directory and naming conventions for schema/data/rollback changes
disable-model-invocation: true
user-invocable: false
---
# SQL Script Naming Standard

## Directory Suggestion
- db/schema
- db/data
- db/rollback

## Naming Rules
- Forward scripts: VYYYYMMDD_NNN_description.sql
- Rollback scripts: RYYYYMMDD_NNN_description.sql
- Use action-oriented names such as create_table, add_index, init_dict.
- Separate schema changes from data initialization when possible.
- High-risk scripts must include execution notes and rollback guidance.