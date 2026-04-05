# Backend Rules / 后端规则

## Tech baseline
- Java 17+
- Spring Boot 3.x
- MyBatis-Plus
- Pragmatic DDD

## Pragmatic DDD boundary
- Use richer domain modeling where business complexity justifies it.
- For simple CRUD, avoid unnecessary aggregates or abstraction.
- Keep layering explicit: interface, application, domain, infrastructure.

## Layer responsibilities
- Interface: controller + request/response DTO + boundary handling
- Application: orchestration, transaction, command/query coordination
- Domain: business rules, invariants, state transitions
- Infrastructure: mapper, DO, SQL, external integration

## Hard constraints
- No business rules in controllers, DTOs, mapper interfaces, SQL mapping, or DO classes.
- No MyBatis-Plus leakage into API contracts or meaningful domain abstractions.
- Controllers stay thin.
- Transactions belong in the application layer unless there is a very explicit reason otherwise.
