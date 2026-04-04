---
name: naming-convention-standard
description: Naming rules for packages, classes, methods, DTOs, DOs, repositories, and SQL-related components
disable-model-invocation: true
user-invocable: false
---
# Naming Convention Standard / 命名规范

## Package Rules / 包命名
- Use lowercase package names / 包名全小写
- Organize by layer and business domain / 按分层与业务域组织
- Avoid vague names like util2, temp, misc / 避免模糊命名

## Class Naming Rules / 类命名
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

## Method Naming Rules / 方法命名
- Use explicit business-oriented names / 使用明确的业务语义命名
- Avoid vague names like handleData, process, doStuff / 避免模糊命名
