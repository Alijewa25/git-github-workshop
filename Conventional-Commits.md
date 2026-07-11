# Conventional Commits

## Introduction

Conventional Commits is a standard for writing clear and consistent commit messages.

It makes project history easier to understand, improves collaboration, and supports automated versioning and changelog generation.

---

## Commit Format

<type>: <short description>

Example:

feat: add user authentication
fix: resolve navbar alignment issue
docs: update installation guide

---

## Common Commit Types

### feat

A new feature.

Example:

feat: add dark mode

---

### fix

A bug fix.

Example:

fix: prevent duplicate login requests

---

### docs

Documentation changes only.

Example:

docs: update README

---

### style

Formatting changes that do not affect code behavior.

Example:

style: format CSS files

---

### refactor

Code improvements without changing functionality.

Example:

refactor: simplify authentication logic

---

### test

Adding or updating tests.

Example:

test: add login unit tests

---

### chore

Maintenance tasks.

Example:

chore: update dependencies

---

### perf

Performance improvements.

Example:

perf: optimize database queries

---

### build

Changes affecting build tools.

Example:

build: update webpack configuration

---

### ci

Continuous Integration changes.

Example:

ci: update GitHub Actions workflow

---

## Scope (Optional)

You can specify the affected area.

Example:

feat(auth): add Google login

fix(api): handle timeout errors

docs(readme): update screenshots

---

## Breaking Changes

Use ! after the type.

Example:

feat!: redesign authentication system

Or:

BREAKING CHANGE: authentication API has changed.

---

## Good Examples

feat: add user profile page

fix: correct mobile layout

docs: update contributing guide

refactor: simplify payment service

test: add API integration tests

---

## Bad Examples

update

final

test

asdf

123

---

## Benefits

- Clear project history
- Easier code reviews
- Automatic changelog generation
- Better collaboration
- Professional development workflow

---

## Summary

Conventional Commits provide a simple and consistent way to write commit messages. Following this standard improves readability, collaboration, and long-term project maintenance.
