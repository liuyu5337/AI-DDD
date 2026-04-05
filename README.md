# AI-DDD Claude Package (Enhanced)

This package is an enhanced `.claude/` template rebuilt from the public repository structure you shared and then upgraded with an explicit `rules/` governance layer.

## What is included
- revised `CLAUDE.md`
- revised `agents/`
- full `skills/` directory skeleton aligned with your current naming
- new `rules/` directory for global governance
- selected `checklists/`, `examples/`, and `templates/`

## Why this version
Your current design already has a good separation between:
- **agents** = task roles
- **skills** = reusable capability/rule bundles

The main gap was:
- many global constraints were still living inside skills
- there was no explicit **rules layer** to act as repository-wide policy

This package adds that missing layer and makes the precedence explicit.

## Suggested load / precedence
1. `CLAUDE.md`
2. `rules/*.md`
3. `agents/*.md`
4. `skills/**/SKILL.md`
5. task-specific templates / checklists / examples

## Recommended workflow
- `/plan-feature`
- `/design-api`
- `/springboot-ddd-module-scaffold`
- `/implement-backend`
- `/prepare-sql-change`
- `/frontend-module-scaffold`
- `/implement-frontend`
- `/run-test-check`
- `/review-changes`
- `/security-check`
- `/write-tech-doc`
- `/commit-pr-standard`
