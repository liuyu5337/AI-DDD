# AI-DDD Repository Contract / 仓库级约定

This repository targets:

- Spring Boot 3.x + Java 17 + MyBatis-Plus
- Vue 3 + Element Plus
- OpenAPI First
- Pragmatic DDD
- SQL-script-based DB changes
- JUnit 5 + Vitest + Vue Test Utils

## Precedence / 优先级

When instructions appear in multiple places, use this order:

1. Explicit user task / 用户当前任务
2. This `CLAUDE.md`
3. `.claude/rules/*.md`
4. Selected agent definition
5. Selected skill definition
6. Templates, checklists, examples

## Boundary of each layer / 分层边界

### Rules
`rules/` are the single source of truth for repository-wide governance.

They define:

- global MUST / MUST NOT
- cross-role expectations
- stable engineering constraints
- shared output conventions where necessary

Rules do **not** define role ownership or long task prompts.

### Agents
`agents/` define:

- role responsibility
- decision focus
- handoff expectations
- required output shape

Agents must not restate repository-wide governance in full.
They may reference the rules and emphasize role-specific risk points.

### Skills
`skills/` define:

- execution methods
- step-by-step checklists
- templates / examples
- user-invocable entry points

Skills must not become a second copy of the rules.
When a rule already exists, a skill should reference it and turn it into an execution checklist.

## Working style / 工作方式

- Use Chinese for daily collaboration when convenient.
- Keep code identifiers, API names, package names, and technical keywords stable in English.
- Keep changes scoped and traceable.
- Prefer compatibility-preserving changes unless the task explicitly allows breaking changes.
- Update tests and docs when behavior, API, SQL, setup, or usage changes.
- Never claim something was implemented, tested, or migrated unless it actually was.

## Suggested workflow / 推荐工作流

1. `/plan-feature`
2. `/design-api`
3. `/springboot-ddd-module-scaffold`
4. `/implement-backend`
5. `/prepare-sql-change`
6. `/frontend-module-scaffold`
7. `/implement-frontend`
8. `/run-test-check`
9. `/review-changes`
10. `/security-check`
11. `/write-tech-doc`
12. `/commit-pr-standard`

## Rules to check / 关键规则索引

- `rules/engineering-rules.md`
- `rules/api-contract-rules.md`
- `rules/backend-rules.md`
- `rules/frontend-rules.md`
- `rules/database-rules.md`
- `rules/security-rules.md`
- `rules/response-error-rules.md`
- `rules/logging-audit-rules.md`
- `rules/testing-rules.md`
- `rules/naming-rules.md`
- `rules/docs-rules.md`
- `rules/delivery-rules.md`
