---
name: branching-release-policy
description: Propose or enforce a pragmatic branching and release policy for feature development, bug fixing, hotfix, and release preparation in this project
context: fork
agent: planner
disable-model-invocation: true
---
Provide branching and release guidance for the following scenario or project setup / 为以下场景提供分支与发布策略建议:

$ARGUMENTS

Project expectations / 项目期望:
- Keep the branching model pragmatic and not overly complex
- Make feature, bugfix, hotfix, release, develop, and main usage explicit
- Keep merge-back rules clear
- Include release and rollback considerations when relevant

You must generate / 你必须生成:
1. Recommended branch naming
2. Branch usage rules
3. Merge strategy guidance
4. Release branch guidance
5. Hotfix process guidance
6. Tagging/versioning suggestions
7. Rollback and back-merge notes

Hard constraints / 强约束:
- Do not propose an overly heavy workflow for a small or medium team
- Keep rules explicit and executable
- Distinguish daily development flow from production hotfix flow
- Make back-merge requirements clear

Required output format / 输出格式:
- branch model summary
- naming rules
- merge rules
- release flow
- hotfix flow
- tagging notes
- rollback notes
