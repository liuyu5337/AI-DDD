# Backend Rules

## Tech baseline
- Java 17+
- Spring Boot 3.x
- MyBatis-Plus
- pragmatic DDD

## Layering
- Interface layer: controller + request/response DTO + external boundary handling
- Application layer: orchestration, transaction, command/query coordination
- Domain layer: business rules, invariants, state transitions
- Infrastructure layer: mapper, DO, persistence, remote integration

## Hard constraints
- controllers stay thin
- no heavy business logic in controller / DTO / mapper / DO
- MyBatis-Plus details stay in infrastructure
- domain modeling should match complexity; do not over-model trivial CRUD
- transaction boundaries should usually stay in application layer
- explicit mapping between DTO / domain / persistence objects

## Quality defaults
- new write actions should consider idempotency
- sensitive actions should consider audit logging
- errors should use global handling
- meaningful behavior changes should add or update tests
