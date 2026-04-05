# AI-DDD v0.0.6 rules-ready package

This package is rebuilt from the public `v0.0.6` structure of `liuyu5337/AI-DDD`, and keeps the original style:

- Agents: English filename + English `name`
- Skills: directory-based `SKILL.md`
- Daily interaction: Chinese recommended
- Mixed Chinese + English wording where clarity helps

## What changed

This package adds a dedicated `rules/` layer and makes boundaries explicit:

- `CLAUDE.md`: repository-level contract and precedence
- `rules/`: global repository governance only
- `agents/`: role responsibilities, decision focus, required outputs
- `skills/`: execution methods, checklists, templates, and command wrappers

## Boundary contract

- Do **not** duplicate the same MUST / MUST NOT across `rules`, `agents`, and `skills`.
- Global constraints live in `rules`.
- Agents tell Claude **who should do what**.
- Skills tell Claude **how to do that kind of work** or provide a user-invocable entry.

## How to use

1. Copy `.claude/` into your repository root.
2. If Finder does not show hidden folders, inspect `claude/`.
3. Use the suggested workflow in `.claude/CLAUDE.md`.
