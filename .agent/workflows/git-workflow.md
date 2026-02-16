---
description: Git and GitHub CLI workflow — use git for local ops, gh for remote ops
---

# Git & GitHub CLI Workflow

## Core Principle

- **Local operations** → use `git`
- **Remote operations** → use `gh` (GitHub CLI)

## Local Operations (use `git`)

Use `git` for anything that touches the local repository:

1. **Staging changes**: `git add`
2. **Committing**: `git commit -m "message"`
3. **Branching**: `git branch`, `git checkout`, `git switch`
4. **Merging locally**: `git merge`
5. **Viewing history**: `git log`
6. **Diffing**: `git diff`
7. **Stashing**: `git stash`
8. **Tagging**: `git tag`
9. **Resetting / reverting**: `git reset`, `git revert`

## Remote Operations (use `gh`)

Use `gh` for anything that interacts with GitHub remotely:

1. **Creating repos**: `gh repo create`
2. **Cloning repos**: `gh repo clone`
3. **Pull requests**: `gh pr create`, `gh pr merge`, `gh pr list`
4. **Issues**: `gh issue create`, `gh issue list`, `gh issue close`
5. **Releases**: `gh release create`, `gh release list`
6. **Viewing repo info**: `gh repo view`
7. **Forking**: `gh repo fork`
8. **GitHub Actions**: `gh run list`, `gh run view`
9. **Gists**: `gh gist create`, `gh gist list`

## Pushing & Pulling

- **Pushing commits**: use `git push` (sends local commits to remote)
- **Pulling commits**: use `git pull` (fetches and merges remote changes locally)

> These are `git` commands because they originate from the local repo context, even though they interact with a remote.

## Notes

- On Windows (PowerShell), do **not** use `&&` to chain commands — run them as separate commands instead.
