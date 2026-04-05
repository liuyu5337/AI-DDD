# Delivery Rules / 交付与流程规则

## Branch / release / PR
- Use explicit branch names that reflect purpose and scope.
- Keep commit messages semantically clear.
- PR descriptions should mention API, SQL, testing, compatibility, and rollback notes where relevant.
- Do not claim tests passed if they were not run.

## CI expectations
- Run the smallest meaningful verification scope first.
- Do not ignore failing checks without explanation.
- Call out flaky tests, environment blockers, or missing validation explicitly.

## Release mindset
- Prefer reversible changes.
- High-risk changes should include rollback or mitigation notes.
- Large releases should identify compatibility and rollout concerns in advance.
