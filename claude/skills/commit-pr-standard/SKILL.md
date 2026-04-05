---
name: commit-pr-standard
description: Generate standardized commit messages, PR titles, PR descriptions, and change summaries for completed work in this project
context: fork
agent: docs-writer
disable-model-invocation: true
---

Prepare commit and PR materials for the following completed change / 为以下已完成改动生成提交与 PR 材料:
$ARGUMENTS

Project expectations / 项目期望:
- use conventional commit style for commit messages
- keep module scope explicit when possible
- include API, SQL, testing, compatibility, and rollback notes when relevant
- keep descriptions concise but review-friendly

You must generate / 你必须生成:
1. recommended commit message candidates
2. recommended PR title candidates
3. PR description draft
4. change summary
5. API impact notes
6. SQL impact notes
7. test summary
8. risk and compatibility notes
9. rollback notes
