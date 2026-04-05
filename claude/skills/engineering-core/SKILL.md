---
name: engineering-core
description: Shared engineering constraints and delivery rules for this project
disable-model-invocation: true
user-invocable: false
---

# Engineering Core / 工程核心规则

## General Rules / 通用规则
- Understand the task before editing / 修改前先理解任务
- Keep changes minimal and scoped / 变更要小而聚焦
- Prefer consistency with the existing codebase / 优先保持与现有代码风格一致
- Do not introduce unrelated refactors / 不要引入无关重构
- Do not present pseudo code as complete implementation / 不要把伪代码当成完成实现

## Delivery Rules / 交付规则
- Identify affected files/modules before editing / 先识别影响范围
- Preserve backward compatibility unless explicitly allowed / 默认保持兼容
- Update tests for meaningful behavior changes / 有意义行为变化要补测试
- Update docs when API, behavior, SQL, setup, or usage changes / 接口、行为、SQL、配置、使用方式变化要更新文档

## Interaction Language / 交互语言
- You may work with the user in Chinese / 可以与用户用中文交互
- Keep technical identifiers stable in English / 技术标识保持英文稳定
- Mixed Chinese + English explanations are preferred when clarity improves / 为提高清晰度可采用中英混合说明

## Finish Report / 收尾输出
When finishing work, summarize / 完成时总结:
- changed files
- key decisions
- tests status
- known risks or limitations
