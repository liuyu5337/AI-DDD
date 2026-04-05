---
name: backend-ddd-mybatisplus
description: Pragmatic DDD + Spring Boot 3.x + Java 17 + MyBatis-Plus backend implementation rules
disable-model-invocation: true
user-invocable: false
---

# Backend Pragmatic DDD Rules / 后端务实 DDD 规则

## Tech Baseline / 技术基线
- Java 17+
- Spring Boot 3.x
- MyBatis-Plus

## Pragmatic DDD / 务实 DDD
- Apply rich domain modeling where business complexity exists / 有复杂业务时做领域建模
- For simple CRUD modules, avoid over-modeling / 简单 CRUD 避免过度建模
- Keep layering explicit: interfaces, application, domain, infrastructure / 分层清晰

## Layer Responsibilities / 分层职责
- Interface: controllers, request/response DTOs, external boundary handling
- Application: orchestration, transactions, command/query coordination
- Domain: business rules, invariants, state transitions
- Infrastructure: Mapper, DO, SQL, external integrations

## Hard Constraints / 强约束
- Do not put business rules in controllers, DTOs, Mapper interfaces, or DO classes
- Do not leak MyBatis-Plus wrappers/pages/entities into API contracts / 不要把 MP 类型泄漏到接口层
- Do not let persistence structure dictate API model directly / 不要让表结构直接主导 API 设计
- Do not create unnecessary aggregates for trivial CRUD / 普通 CRUD 不要硬造聚合
- Enforce domain rules where meaningful complexity exists / 有复杂度时必须落实领域规则

## Implementation Expectations / 实现要求
- Keep controllers thin
- Keep application services explicit
- Separate persistence objects from domain concepts when needed / 需要时区分 DO 与领域对象
- Prefer clear naming over abstract naming / 命名优先清晰
