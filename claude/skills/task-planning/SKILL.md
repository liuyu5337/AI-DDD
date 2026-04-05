---
name: task-planning
description: Planning checklist for feature analysis and task decomposition
disable-model-invocation: true
user-invocable: false
---

# Task Planning Method / 任务规划方法

Source of truth / 规则来源:
- `.claude/rules/engineering-rules.md`
- `.claude/rules/delivery-rules.md`

## Planning output should include / 规划输出应包含
1. goal and value
2. scope and non-goals
3. assumptions
4. backend impact
5. frontend impact
6. API impact
7. SQL impact
8. test impact
9. documentation impact
10. risks and execution order

For medium or large tasks, split clearly into:
- API design
- backend implementation
- frontend implementation
- SQL changes
- tests
- documentation
