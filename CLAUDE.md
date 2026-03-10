# CLAUDE.md — AI Assistant Guide for programacion-practicas-seo

This file provides context for AI assistants (Claude and others) working in this repository.

---

## Repository Overview

**Name:** programacion-practicas-seo
**Author:** cmalolara
**Purpose:** Educational practice repository for a SEO programming course, focused on learning Git version control workflows.
**Language:** No programming language — text-based content only.
**Last active:** February 1, 2021

This is a minimal learning repository. Its primary goal is to demonstrate basic Git operations: creating files, making commits, branching, and merging via pull requests.

---

## Directory Structure

```
programacion-practicas-seo/
├── CLAUDE.md               # This file
└── git/                    # All practice content lives here
    ├── .gitignore          # Excludes node_modules
    ├── readme.md           # One-line course description
    └── git-practicas.txt   # Practice text file modified across commits
```

There are no source code directories, build systems, test suites, or configuration files beyond `.gitignore`.

---

## Git Workflow & Conventions

### Branch Strategy

The project uses a simple feature-branch workflow:

- `master` — main/default branch; all stable content lives here
- `feature/<name>` — short-lived branches for isolated changes, merged back via pull request

Example from history: `feature/ejemplo` was branched off master, modified content, then merged via PR #1.

### Commit Message Style

Commits are written in informal, mixed Spanish/English lowercase:

| Commit | Message |
|--------|---------|
| `f1ecd98` | `creacion repo` |
| `842b5ca` | `cambiar a por BB` |
| `daba81a` | `add readme and add gitignore` |
| `3b1d813` | `segunda subida ig` |
| `a97aac4` | `Merge pull request #1 from cmalolara/feature/ejemplo` |

**Convention:** Short, descriptive, lowercase, no period at end. No strict format enforced.

### Pull Request Workflow

Changes are merged into `master` via pull requests. The merge commit message follows GitHub's default format:
```
Merge pull request #<N> from <user>/<branch>
```

---

## File Descriptions

### `git/git-practicas.txt`
A text file used as the practice subject across the commit history. Its content has been modified to demonstrate how Git tracks changes:
- Initial state: empty
- After `cambiar a por BB`: contains `El texto es BB`

### `git/readme.md`
A single-line project description:
```
Repositorio del curso de programacion SEO
```

### `git/.gitignore`
Contains one entry:
```
node_modules
```
Added preemptively even though no Node.js project exists, which is common in course repositories that may evolve.

---

## Development Workflows

### No Build System
There is no build, compile, or bundle step. No `npm`, `yarn`, `make`, or similar tooling is required.

### No Tests
There is no testing infrastructure. No test files, no test runner, no CI/CD pipeline.

### No Dependencies
There are no package managers or dependency files (`package.json`, `requirements.txt`, etc.).

---

## Working in This Repository

### For AI Assistants

- **Keep changes minimal.** This is a simple educational repo; avoid over-engineering.
- **Commit messages** should follow the established style: short, lowercase, informal, Spanish or English.
- **Branch naming:** use `feature/<descriptive-name>` for new work branches, or follow the branch naming pattern provided by the task context.
- **Do not introduce build tooling, frameworks, or dependencies** unless explicitly requested.
- **The `git/` subdirectory** is where all course content lives; place any new practice files there.

### Typical Tasks in This Repo

Common operations expected in a course like this:

1. Creating/editing text files to practice staging and committing
2. Creating feature branches and opening pull requests
3. Demonstrating `git diff`, `git log`, `git status` concepts
4. Practicing merge strategies (fast-forward, squash, merge commit)
5. Resolving simple merge conflicts for learning purposes

---

## Remote Configuration

- **Remote name:** `origin`
- **Remote URL:** `http://local_proxy@127.0.0.1:34931/git/cmalolara/programacion-practicas-seo`

This points to a local proxy, likely a Gitea or similar self-hosted Git instance used in the course environment.

---

## Key Facts Summary

| Property | Value |
|----------|-------|
| Type | Educational / practice |
| Language | None (plain text) |
| Framework | None |
| Package manager | None |
| Testing | None |
| CI/CD | None |
| Primary branch | `master` |
| Branch strategy | Feature branches + PR merge |
| Commit language | Spanish / English mixed |
