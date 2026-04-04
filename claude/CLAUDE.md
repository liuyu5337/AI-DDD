# Project Instructions

## Tech Stack / 技术栈
- Backend: Java 17+, Spring Boot 3.x, MyBatis-Plus
- Frontend: Vue 3 + Element Plus
- API style: OpenAPI First
- Design style: Pragmatic DDD / 务实 DDD
- DB change management: SQL scripts
- Backend tests: JUnit 5
- Frontend tests: Vitest + Vue Test Utils

## Working Language / 工作语言
- Daily interaction with Claude Code: Chinese is fine / 日常交互可直接使用中文
- Agent filenames and skill names stay in English / agent 文件名与 skill 名称保持英文
- Rule bodies prefer mixed Chinese + English for clarity / 规则正文采用中英混合，兼顾稳定性与可读性

## Global Delivery Rules / 全局交付规则
- Understand task scope before editing code / 修改前先理解任务范围
- For medium or large work, plan first / 中大型需求先规划
- For API changes, design contract first / 接口变更先设计合同
- Keep changes minimal, explicit, and reviewable / 变更应小而清晰，便于 review
- Do not claim pseudo code as finished implementation / 不要把伪代码当作完成实现
- Preserve backward compatibility unless explicitly allowed / 除非明确允许，否则保持兼容
- Significant changes must mention test impact and doc impact / 重要改动要说明测试与文档影响

## Backend Rules / 后端规则
- Controllers must stay thin / Controller 保持薄
- Business rules must not live in controllers, DTOs, mappers, or DO classes / 业务规则不能落在 Controller、DTO、Mapper、DO 中
- MyBatis-Plus belongs to infrastructure / MyBatis-Plus 只属于基础设施层
- Use pragmatic DDD: apply domain modeling where business complexity exists / 务实 DDD：有复杂业务才做领域建模
- Simple CRUD modules should not be over-modeled / 简单 CRUD 不要过度建模
- Application layer handles orchestration and transaction boundaries / 应用层负责编排与事务边界
- Domain layer handles rules, invariants, and state transitions / 领域层负责规则、不变量、状态流转
- Infrastructure handles Mapper / DO / SQL / integration details / 基础设施层负责 Mapper、DO、SQL、外部集成实现

## OpenAPI Rules / 接口规则
- Prefer OpenAPI First for new or changed APIs / 新增或变更接口优先 OpenAPI First
- Define request/response DTOs, validation, error model, pagination, compatibility before implementation / 实现前定义请求、响应、校验、错误模型、分页与兼容策略
- Do not expose persistence objects directly / 不要直接暴露持久化对象

## Database Rules / 数据库规则
- DB changes must be delivered as SQL scripts / 数据库变更以 SQL 脚本交付
- Every schema/data change must include rollback or mitigation notes / 每次 schema/data 变更都要有回滚或缓解说明
- Avoid destructive SQL without explicit warning / 破坏性 SQL 必须明确警告
- Index design must be based on query patterns / 索引设计基于查询模式而非拍脑袋

## Frontend Rules / 前端规则
- Use Vue 3 Composition API / 使用 Vue3 Composition API
- Use Element Plus consistently / 统一使用 Element Plus 风格
- Centralize API calls / API 调用集中管理
- Avoid heavy business logic in templates / 模板中避免重业务逻辑
- Make loading/empty/error states explicit / 明确 loading、empty、error 状态
- Prefer reusable components / 优先复用组件

## Testing Rules / 测试规则
- Meaningful behavior changes should be covered by tests / 有意义的行为变化应补测试
- Backend tests use JUnit 5 / 后端使用 JUnit5
- Frontend tests use Vitest + Vue Test Utils / 前端使用 Vitest + Vue Test Utils
- Report what was tested, what passed, and what remains untested / 交付时说明测了什么、通过什么、还缺什么

## Security Rules / 安全规则
- Validate untrusted input / 校验不可信输入
- Do not hardcode secrets / 不要硬编码密钥
- Do not log tokens, passwords, or sensitive data / 不要记录 token、密码或敏感数据
- Sensitive changes should be reviewed by security-reviewer / 安全敏感改动应经过 security-reviewer
- Permission checks must be explicit on sensitive operations / 敏感操作必须有明确权限校验

## Documentation Rules / 文档规则
- Update docs when API, behavior, database, deployment, or usage changes / 接口、行为、数据库、部署、使用方式变化要更新文档
- Documentation must align with actual implementation / 文档必须与实现一致
- Include assumptions, affected files/modules, and known risks / 说明假设、影响范围和已知风险
