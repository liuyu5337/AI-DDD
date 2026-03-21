# DDD Spring Boot Project Skill

## Purpose
Generate code based on DDD layered architecture for Spring Boot projects.

## Required Layers
- interfaces
- application
- domain
- infrastructure

## Generation Rules
- Controller only handles request/response
- Application Service orchestrates use cases
- Domain contains aggregates, entities, value objects, repository interfaces, domain services
- Infrastructure contains persistence PO, mapper, repository implementation, external integrations
- Do not expose domain aggregate directly to API response
- Do not place DTO in domain layer
- Use assembler/convert to transform between layers

## Output Requirements
When generating a module, always output:
1. request/response DTO
2. command/query object
3. application service
4. domain aggregate/entity/value object
5. repository interface
6. repository implementation
7. persistence PO + mapper
8. assembler / convert