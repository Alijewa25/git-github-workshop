# Conventional Commits

> A standardized convention for writing clear, consistent, and meaningful Git commit messages.

---

## Table of Contents

- [What are Conventional Commits?](#what-are-conventional-commits)
- [Why Use Conventional Commits?](#why-use-conventional-commits)
- [Commit Message Structure](#commit-message-structure)
- [Commit Types](#commit-types)
- [Scope](#scope)
- [Breaking Changes](#breaking-changes)
- [Examples](#examples)
- [Best Practices](#best-practices)
- [Common Mistakes](#common-mistakes)
- [Quick Reference](#quick-reference)
- [Summary](#summary)

---

# What are Conventional Commits?

Conventional Commits is a widely adopted specification for writing commit messages in a consistent format.

Using this convention makes Git history easier to read, improves collaboration, and enables automated tools such as changelog generators and semantic versioning.

---

# Why Use Conventional Commits?

| Benefit | Description |
|----------|-------------|
| 📖 Readable History | Makes commit history easier to understand |
| 👥 Better Collaboration | Everyone follows the same structure |
| 🚀 Easier Code Reviews | Reviewers instantly know what changed |
| 🤖 Automation | Supports automatic changelog generation |
| 📦 Semantic Versioning | Works with automated release tools |
| 🔍 Easier Debugging | Quickly locate specific changes |

---

# Commit Message Structure

General format:

```text
<type>(optional-scope): <description>
```

Example:

```bash
feat(auth): add Google authentication
```

---

## Structure Breakdown

| Part | Required | Description |
|------|----------|-------------|
| Type | ✅ | Specifies the type of change |
| Scope | Optional | Indicates the affected module |
| Description | ✅ | Short explanation of the change |

---

# Commit Types

| Type | Purpose | Example |
|------|---------|---------|
| **feat** | Introduce a new feature | `feat: add dark mode` |
| **fix** | Fix a bug | `fix: resolve login error` |
| **docs** | Documentation only | `docs: update README` |
| **style** | Formatting or styling | `style: format CSS files` |
| **refactor** | Improve code without changing behavior | `refactor: simplify authentication` |
| **test** | Add or update tests | `test: add unit tests` |
| **perf** | Improve performance | `perf: optimize database query` |
| **build** | Build system changes | `build: update webpack configuration` |
| **ci** | Continuous Integration changes | `ci: add GitHub Actions workflow` |
| **chore** | Maintenance tasks | `chore: update dependencies` |

---

# Scope

The scope identifies the part of the project affected by the change.

Examples:

```bash
feat(auth): add login API
```

```bash
fix(ui): resolve button alignment
```

```bash
docs(readme): improve installation guide
```

Using scopes is optional but highly recommended for medium and large projects.

---

# Breaking Changes

If a commit introduces incompatible changes, use **!** after the type.

Example:

```bash
feat!: redesign authentication system
```

or

```text
BREAKING CHANGE: Authentication API has changed.
```

---

# Examples

## Good Examples

```bash
feat: add user dashboard
```

```bash
fix: prevent duplicate requests
```

```bash
docs: update installation guide
```

```bash
refactor: simplify payment service
```

```bash
perf: optimize SQL queries
```

---

## Bad Examples

```text
update
```

```text
test
```

```text
final
```

```text
123
```

```text
asdf
```

These commit messages provide little or no useful information.

---

# Best Practices

✅ Write commit messages in the imperative mood.

Good:

```text
Add login page
```

Bad:

```text
Added login page
```

---

✅ Keep the first line concise.

Recommended length:

**Less than 50 characters**

---

✅ One commit should represent one logical change.

Good:

```
Add login form

Add validation

Connect API
```

Bad:

```
Complete project
```

---

✅ Make commits frequently.

Small commits are easier to review, revert, and debug.

---

✅ Use meaningful commit messages.

Every commit should clearly explain **what changed**.

---

# Common Mistakes

| ❌ Avoid | ✅ Prefer |
|----------|-----------|
| update | feat: add profile page |
| final | fix: resolve navbar bug |
| test | docs: update README |
| asdf | refactor: simplify API |
| commit | chore: update dependencies |

---

# Quick Reference

| Situation | Commit Type |
|------------|------------|
| New feature | feat |
| Bug fix | fix |
| Documentation | docs |
| Refactoring | refactor |
| Styling | style |
| Tests | test |
| Performance | perf |
| Build system | build |
| CI/CD | ci |
| Maintenance | chore |

---

# Summary

Conventional Commits provide a standardized way to write Git commit messages.

Following this convention helps maintain a clean project history, improves collaboration, simplifies debugging, and supports automated development workflows.
