---
name: backend-ddd-mybatisplus
description: Pragmatic DDD + Spring Boot 3.x + Java 17 + MyBatis-Plus backend execution method
disable-model-invocation: true
user-invocable: false
---

# Backend Execution Method / 后端实现方法

Source of truth / 规则来源:
- `.claude/rules/backend-rules.md`
- `.claude/rules/api-contract-rules.md`
- `.claude/rules/database-rules.md`

## Decision flow / 决策流程
1. Decide whether the requirement is simple CRUD or domain-heavy logic.
2. If simple CRUD, keep the model light and explicit.
3. If business invariants or state transitions matter, model them in domain objects or domain services.
4. Keep controller -> application -> domain -> infrastructure responsibilities clear.
5. Keep mapper / DO / query wrappers inside infrastructure.

## Implementation pattern / 实现套路
- Request DTO -> application command/query
- Application service orchestrates transaction and collaboration
- Domain handles rules where complexity exists
- Repository hides persistence details
- Response DTO is assembled at boundary

## Delivery reminders / 交付提醒
- Check API contract impact.
- Check SQL impact.
- Check audit/logging impact.
- Add or update JUnit 5 tests.
