---
name: commit-pr-standard
description: Generate standardized commit messages, PR titles, PR descriptions, and change summaries for completed work in this project
context: fork
agent: docs-writer
disable-model-invocation: true
---
Prepare commit and PR materials for the following completed change:

$ARGUMENTS

Project expectations:
- Use conventional commit style for commit messages
- Keep module scope explicit when possible
- Include API, SQL, testing, compatibility, and rollback notes when relevant
- Keep descriptions concise but review-friendly

You must generate, when appropriate:
1. Recommended commit message candidates
2. Recommended PR title candidates
3. PR description draft
4. Change summary
5. API impact notes
6. SQL impact notes
7. Test summary
8. Risk and compatibility notes
9. Rollback notes

Hard constraints:
- Do not claim tests passed if they were not run.
- Do not invent SQL changes, API changes, or rollback steps.
- Keep commit messages semantically clear.
- Keep PR description aligned with actual implementation.
- Explicitly mention missing verification or open risks.

Required output format:
- commit message options
- PR title options
- PR description draft
- risk notes
- rollback notes