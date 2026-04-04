---
name: frontend-module-scaffold
description: Scaffold a Vue 3 + Element Plus business module aligned with centralized API calls, unified page patterns, and agreed backend contracts
context: fork
agent: frontend-coder
disable-model-invocation: true
---
Scaffold a frontend module for the following business requirement / 为以下业务需求生成前端模块骨架:

$ARGUMENTS

Project constraints / 项目约束:
- Vue 3
- Composition API
- Element Plus
- Frontend-backend separation
- Centralized API request modules
- Stable response envelope handling
- Vitest + Vue Test Utils

You must generate or propose / 你应生成或提出:
1. Module responsibility summary
2. Recommended directory structure
3. Page structure for search area, action area, table area, and pagination area
4. API request module skeleton
5. Types or interface skeletons if appropriate
6. Search form model and form-item suggestions
7. Table column definitions
8. Create/edit dialog or drawer skeleton
9. Detail drawer/page skeleton where relevant
10. Composable or hooks suggestions for page logic extraction
11. Vitest + Vue Test Utils test skeletons
12. Notes about API assumptions, loading/empty/error states, and reusable component opportunities

Hard constraints / 强约束:
- Do not place heavy business logic in templates
- Do not scatter API requests across unrelated components
- Keep index pages focused on composition
- Prefer reusable components when patterns repeat
- Keep loading, empty, and error states explicit
- Keep field names aligned with the API contract or document mapping clearly
- Do not silently invent backend fields or behaviors

Required output format / 输出格式:
- module summary
- directory structure
- API module draft
- page/component scaffold list
- sample component skeletons
- test skeleton plan
- risks and follow-up notes
