# Spring Boot API Generator Skill

## Purpose
Generate enterprise-grade Spring Boot API code with:
- OpenAPI3 annotations
- DTO request/response models
- Controller / Service / Mapper / Entity skeleton
- validation
- unified ApiResponse
- exception handling
- audit / idempotency / auth placeholders

适用于：
- Spring Boot 3.x
- REST API
- MyBatis-Plus / JPA /Mybatis 风格项目
- 企业级系统集成场景

---

## Generation Rules

### 1. Package Structure
生成代码时优先使用以下分层：
- controller
- service
- service.impl
- dto.request
- dto.response
- entity
- mapper
- convert

### 2. API Style
必须遵循：
- RESTful URL
- 统一 `/api/v1/{module}` 前缀
- 统一返回 `ApiResponse<T>`
- 分页返回 `ApiResponse<PageResponse<T>>`

### 3. OpenAPI3
必须添加：
- `@Tag`
- `@Operation`
- `@Schema`
- `@Parameter`（必要时）
- `@SecurityRequirement(name = "bearerAuth")`（受保护接口）

### 4. DTO Rules
- Request 和 Response 分离
- Request 类名：`CreateXxxRequest` / `UpdateXxxRequest` / `QueryXxxRequest`
- Response 类名：`XxxResponse`
- 不直接暴露 Entity 给前端
- DTO 字段使用 `@Schema(description = "...")`

### 5. Validation Rules
Request DTO 必须按需使用：
- `@NotNull`
- `@NotBlank`
- `@Size`
- `@Pattern`
- `@Valid`

### 6. Controller Rules
Controller 只做：
- 参数接收
- 参数校验
- 调用 Service
- 返回 ApiResponse
不得写复杂业务逻辑

### 7. Service Rules
Service 负责：
- 核心业务逻辑
- 权限/状态/流程校验
- 调用 mapper/repository
- 事务边界

### 8. Security Rules
如果接口为登录后可访问：
- 预留 `@PreAuthorize(...)`
- 从上下文获取 userId / tenantId / orgId
- 不允许从前端直接传 userId 作为可信身份

### 9. Audit Rules
新增、修改、删除、导出接口：
- 添加 `@AuditLog`
- 审计内容包括 action / module / bizType

### 10. Idempotency Rules
以下场景优先考虑 `@Idempotent`：
- 提交申请
- 创建单据
- 重提
- 支付/确认类操作

### 11. Error Handling
- 业务异常使用 `BizException`
- 不直接抛裸 RuntimeException
- Controller 不直接 try/catch 业务异常，交给全局异常处理

### 12. Compatibility
- 默认向后兼容
- 新增字段允许
- 删除字段需谨慎并提示版本影响

---

## Output Requirements
当生成接口代码时，必须同时输出：
1. API path
2. DTO list
3. files generated
4. risk notes
5. TODO items for auth/audit/idempotency if not fully implemented