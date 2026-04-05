# Database Rules

## Change management
- schema changes use reviewed SQL scripts
- explain scope, risk, rollback, and data impact
- avoid destructive SQL without explicit warning
- distinguish schema SQL and data fix SQL

## Modeling
- naming must be clear and stable
- nullability, defaults, constraints, and unique keys should be deliberate
- indexes should come from real query patterns
- keep persistence model aligned with pragmatic DDD boundaries

## Delivery output
For each SQL change mention:
- affected tables
- DDL / DML intent
- index impact
- compatibility risk
- rollback or mitigation
