---
name: backend-ddd-mybatisplus
description: Pragmatic DDD + Spring Boot 3.x + Java 17 + MyBatis-Plus backend implementation rules
disable-model-invocation: true
user-invocable: false
---
# Backend Pragmatic DDD Rules

## Tech Baseline
- Java 17+
- Spring Boot 3.x
- MyBatis-Plus

## Pragmatic DDD Rules
- Apply rich domain modeling where business complexity exists.
- For simple CRUD modules, avoid over-modeling.
- Keep layering explicit: interfaces, application, domain, infrastructure.

## Layer Responsibilities
- Interface: controllers, request/response DTOs, external boundary handling
- Application: use-case orchestration, transaction boundaries, command/query coordination
- Domain: business rules, invariants, state transitions, core domain behavior
- Infrastructure: MyBatis-Plus Mapper, DO classes, SQL implementation, external integrations

## Hard Constraints
- Do not put business rules in controllers, DTOs, Mapper interfaces, or DO classes.
- Do not leak MyBatis-Plus wrappers/pages/entities into API contracts.
- Do not let persistence structure dictate API model directly.
- Do not create unnecessary aggregates for trivial CRUD.
- Do enforce domain rules where there is meaningful complexity.

## Implementation Expectations
- Keep controllers thin.
- Keep application services explicit.
- Keep persistence objects separate from domain concepts when needed.
- Prefer clear naming over abstract naming.