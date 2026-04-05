# Database Rules / 数据库规则

## Delivery format
- Schema and data changes are delivered as SQL scripts.
- Distinguish schema change, data change, execution order, rollback, and compatibility notes.

## Risk control
- Destructive SQL requires explicit warning.
- Explain rollback or mitigation strategy.
- Consider large-table impact, index rebuild cost, lock risk, and execution window where relevant.
- Index design must come from real query patterns.

## Modeling boundary
- Keep persistence DO separate from API DTO and from domain concepts when necessary.
- Do not let persistence shortcuts distort business semantics.
## Naming
- SQL script names must be sortable, explicit, and review-friendly.
- Include change intent in the file name.
