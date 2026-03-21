# Project Rules

## Project overview
- This is an enterprise application with backend, frontend, and docs modules.
- Backend uses Spring Boot 3.x, frontend uses Vue 3 + Element Plus.
- Prefer small, reversible changes.

## Engineering rules
- Do not rename modules or move directories unless explicitly required.
- Do not introduce new frameworks without justification.
- Keep API contracts backward compatible unless task says otherwise.
- Write or update tests when changing behavior.
- Update docs when changing public APIs, configs, or scripts.

## Code style
- Backend: prefer clear service boundaries, DTO/VO separation, no giant methods.
- Frontend: keep API calls centralized, avoid business logic inside components when possible.
- Config: never hardcode secrets, tokens, or passwords.

## Delivery format
- Always report:
  1. what changed
  2. affected files
  3. risks
  4. follow-up suggestions

## Architecture: DDD (Domain-Driven Design)

本项目必须遵循 DDD 分层：

### Layers

- interfaces（controller）（接口层）
- application（application service）（应用层）
- domain（entity / aggregate / repository interface）（领域层）
- infrastructure（repository impl / db / external api）（基础设施层）

### Hard Rules(强制规则)：

- Service 分为：
  - Application Service（编排）
  - Domain Service（业务规则）
- Controller 只调用 application service
- Application service 不包含复杂业务规则
- 业务规则必须在 domain 层
- Repository interface 在 domain，impl 在 infrastructure(Repository 接口在 domain，实现在 infrastructure)
- Repository 接口定义在 domain
- Repository 实现放在 infrastructure
- Application Service 负责流程编排
- Domain Service 负责核心业务规则
- PO 仅用于 persistence，不允许向上层泄漏

- 禁止：
  - Controller 写业务逻辑
  - Service 直接写 SQL
  - Controller 不允许写业务逻辑
  - Entity/Aggregate 直接返回给前端
  - Entity 直接暴露给 Controller
  - DTO 进入 domain 层

### Naming

- XxxApplicationService
- XxxDomainService
- XxxRepository
- XxxEntity
- XxxAggregate