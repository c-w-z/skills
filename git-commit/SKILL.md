---
name: git-commit
description: Use when committing changes or asked to commit.
---

# Message
Conventional Commits: `<type>(<scope>)!: <description>`.
- type: feat, fix, docs, style, refactor, perf, test, build, ci, chore, revert.
- `!` marks a breaking change.

# Mechanics
eval `commit` namespace available → `commit.draft()` / `d.commit()`; otherwise `git add` / `git commit`.

# Safety
- NEVER change git config.
- NEVER skip hooks (`--no-verify`) unless asked.
- Hook fails → fix, then make a NEW commit; NEVER amend.
- NEVER push, force-push, hard-reset, or run other destructive commands without explicit confirmation.

# After
Report the short hash and branch.
