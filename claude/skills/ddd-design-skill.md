# DDD Design Skill

## Purpose
Guide domain-driven design implementation.

---

## 1. Entity vs Value Object

- Entity：有 ID，有生命周期
- Value Object：无 ID，不可变

---

## 2. Aggregate

- 每个 aggregate 有 root（Aggregate Root）
- 外部只能通过 root 访问
- 保证一致性边界

---

## 3. Repository

- 定义在 domain 层
- 只面向 aggregate
- 不暴露 DB 细节

---

## 4. Application Service

负责：
- 编排流程（orchestration）
- 调用 domain
- 调用 repository

不负责：
- 核心业务规则

---

## 5. Domain Service

用于：
- 跨 entity 的业务逻辑
- 复杂规则

---

## 6. Anti-patterns（禁止）

- ❌ Entity 当 DTO
- ❌ Service 写 SQL
- ❌ Controller 写业务逻辑
- ❌ 跨 aggregate 修改数据