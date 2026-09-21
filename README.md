# test-1

A scratch repository for practicing Git. It contains no application code — just a few
small text files that exist so there is something to commit, amend, branch, and diff.

## Contents

| File | What it is |
| --- | --- |
| `f1.txt` | Built up one line at a time (`a`, `b`, `c`, `d`), one commit per line — useful for practicing `git log`, `git diff`, and `git revert` against a linear history. |
| `f2.txt` | A single line of comma-separated values, added in its own commit. |
| `f3.txt` | A one-line file, the most recent addition. |

## Getting started

```bash
git clone https://github.com/Glorykim03/test-1.git
cd test-1
```

## Practicing

Nothing here needs to be built or installed, so any Git command is safe to try.
A few starting points:

```bash
# See how f1.txt grew, one commit at a time
git log --oneline --stat

# See what a single commit changed
git show <commit>

# Compare your working copy against the last commit
git diff
```

Experiment on a branch so `main` stays as a clean reference point:

```bash
git switch -c practice
# ...make changes, commit, merge, rebase, reset...
git switch main
```

If an experiment goes sideways, `git reset --hard origin/main` puts the working tree
back to the published state. That command discards uncommitted work, which is exactly
what you want in a scratch repo and never what you want in a real one.

## Conventions

Commits so far use short, imperative messages (`add c`, `create f3.txt`). Korean
messages appear too (`f2.txt 만들기`) — either language is fine here.
