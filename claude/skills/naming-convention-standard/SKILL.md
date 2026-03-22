---
name: naming-convention-standard
description: Naming rules for packages, classes, methods, DTOs, DOs, repositories, and SQL-related components
disable-model-invocation: true
user-invocable: false
---
# Naming Convention Standard

## Package Rules
- Use lowercase package names.
- Organize by layer and business domain.
- Avoid vague package names like util2, temp, misc.

## Class Naming Rules
- Controllers: XxxController
- Application services: XxxAppService
- Domain services: XxxDomainService
- Repositories: XxxRepository
- Repository implementations: XxxRepositoryImpl
- Persistence objects: XxxDO
- Mappers: XxxMapper
- Request DTOs: XxxCreateRequest / XxxQueryRequest
- Response DTOs: XxxDetailResponse / XxxPageResponse
- Converters/assemblers: XxxAssembler / XxxConverter

## Method Naming Rules
- Use explicit business-oriented names.
- Avoid vague names like handleData, process, doStuff.