# Project Instructions

## Tech Stack
- Backend: Java 17+, Spring Boot 3.x, MyBatis-Plus
- Frontend: Vue 3 + Element Plus
- Architecture: Frontend-backend separation
- API style: OpenAPI First
- Design style: Pragmatic DDD
- DB change management: SQL scripts
- Backend tests: JUnit 5
- Frontend tests: Vitest + Vue Test Utils

## Global Delivery Rules
- Always understand task scope before editing code.
- For medium or large work, plan first.
- For API changes, design the contract first.
- Keep changes minimal, explicit, and reviewable.
- Do not claim incomplete or pseudo code as finished implementation.
- Preserve backward compatibility unless the task explicitly allows breaking changes.
- Significant changes must include test impact and documentation impact.

## Backend Rules
- Controllers must stay thin.
- Business rules must not live in controllers, DTOs, mappers, or persistence DO classes.
- MyBatis-Plus belongs to infrastructure, not domain.
- Use pragmatic DDD: apply domain modeling where business complexity exists.
- Simple CRUD modules should not be over-modeled.
- Application layer handles use-case orchestration and transaction boundaries.
- Domain layer handles core business rules, invariants, and state transitions.
- Infrastructure layer handles Mapper/DO/SQL/integration details.

## OpenAPI Rules
- Prefer OpenAPI First for new or changed APIs.
- Define request/response DTOs, validation rules, error models, pagination, and compatibility strategy before implementation.
- Do not expose persistence objects directly as API contracts.

## Database Rules
- Database changes must be delivered as SQL scripts.
- Every schema/data change must include rollback or mitigation notes.
- Avoid destructive SQL without explicit warning.
- Index design must be based on query patterns, not guesswork.

## Frontend Rules
- Use Vue 3 Composition API.
- Use Element Plus consistently.
- Centralize API calls.
- Avoid heavy business logic in templates.
- Keep loading/empty/error states explicit.
- Prefer reusable components over duplicated page logic.

## Testing Rules
- Meaningful behavior changes should be covered by tests.
- Backend tests use JUnit 5.
- Frontend tests use Vitest + Vue Test Utils.
- Report what was tested, what passed, and what remains untested.

## Security Rules
- Validate untrusted input.
- Do not hardcode secrets.
- Do not log tokens, passwords, or sensitive data.
- Security-sensitive changes should be reviewed by security-reviewer.
- Permission checks must be explicit on sensitive operations.

## Documentation Rules
- Update technical docs when API, behavior, database, deployment, or usage changes.
- Documentation must align with actual implementation.
- Include assumptions, affected files/modules, and known risks.