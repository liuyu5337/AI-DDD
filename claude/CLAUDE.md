# Project Instructions

> Rules precedence / 规则优先级：`CLAUDE.md` > `rules/*.md` > `agents/*.md` > `skills/**/SKILL.md`


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

## Priority / 优先级
When multiple instructions exist, follow this order / 当存在多层指令时，按以下优先级执行:
1. This `CLAUDE.md`
2. Files under `.claude/rules/`
3. Agent instructions under `.claude/agents/`
4. Skill instructions under `.claude/skills/`
5. Task-specific checklists, templates, and examples

## Global Delivery Rules / 全局交付规则
- Understand task scope before editing code / 修改前先理解任务范围
- For medium or large work, plan first / 中大型需求先规划
- For API changes, design contract first / 接口变更先设计合同
- Keep changes minimal, explicit, and reviewable / 变更应小而清晰，便于 review
- Do not claim pseudo code as finished implementation / 不要把伪代码当作完成实现
- Preserve backward compatibility unless explicitly allowed / 除非明确允许，否则保持兼容
- Significant changes must mention test impact and doc impact / 重要改动要说明测试与文档影响
- New write operations should consider idempotency, auditability, and permission checks / 新增写操作需考虑幂等、审计、权限
- SQL changes must mention rollback or mitigation / SQL 变更必须说明回滚或缓解方案

## Rule Loading Reminder / 规则加载提醒
Always follow repository rules under `.claude/rules/` as global governance documents.
尤其在以下场景必须优先参考 rules:
- API 设计
- 安全与权限
- 数据库变更
- 日志与审计
- 测试与发布
- 命名与目录规范

## Finish Report / 收尾输出
When finishing work, summarize / 完成时总结:
- changed files
- key decisions
- test status
- doc impact
- SQL impact
- known risks or limitations
