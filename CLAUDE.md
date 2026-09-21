# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A scratch repository for practicing Git (`origin`: `github.com/Glorykim03/test-1`). It holds a few small `.txt` files (`f1.txt`–`f3.txt`) and a `README.md`; there is no application code, build system, linter, or test suite, so there are no such commands to run.

## Working here

- The point of the repo is the commit history, not the file contents. `f1.txt` is deliberately grown one line per commit (`a`, `add b`, `add c`, `add d`) to give a linear history to practice `log`/`diff`/`revert` against. Don't squash, rewrite, or "clean up" existing history unless asked.
- Keep `main` as a clean reference point; do experiments on a branch (`git switch -c <name>`).
- Commit messages are short and imperative (`add c`, `create f3.txt`); Korean messages are also used and are fine.
- Only commit or push when asked. Note that `git reset --hard origin/main` discards uncommitted work — fine for this repo's purpose, but confirm before running it.
