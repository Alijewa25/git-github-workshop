# Contributing Guide

> This guide explains how to contribute to the project effectively using Git and GitHub best practices. Whether you are fixing a bug, adding a new feature, or improving documentation, following these guidelines helps maintain a clean and organized repository.

---

## Table of Contents

- [Why Contribute?](#why-contribute)
- [Contribution Workflow](#contribution-workflow)
- [Prerequisites](#prerequisites)
- [Fork the Repository](#fork-the-repository)
- [Clone the Repository](#clone-the-repository)
- [Create a Branch](#create-a-branch)
- [Make Changes](#make-changes)
- [Commit Your Changes](#commit-your-changes)
- [Push to GitHub](#push-to-github)
- [Open a Pull Request](#open-a-pull-request)
- [Code Review](#code-review)
- [After Your Pull Request is Merged](#after-your-pull-request-is-merged)
- [Best Practices](#best-practices)
- [Common Mistakes](#common-mistakes)
- [Quick Reference](#quick-reference)
- [Summary](#summary)

---

# Why Contribute?

Open-source software grows through collaboration.

Contributors help projects by:

- 🐞 Fixing bugs
- ✨ Adding new features
- 📖 Improving documentation
- ⚡ Optimizing performance
- 🧪 Writing tests
- 💡 Suggesting improvements

Every contribution, regardless of size, adds value to the project.

---

# Contribution Workflow

```text
Fork Repository
        │
        ▼
Clone Repository
        │
        ▼
Create Branch
        │
        ▼
Write Code
        │
        ▼
Commit Changes
        │
        ▼
Push Branch
        │
        ▼
Open Pull Request
        │
        ▼
Code Review
        │
        ▼
Merge
```

---

# Prerequisites

Before contributing, make sure you have:

- Git installed
- A GitHub account
- Basic Git knowledge
- Access to the project repository

---

# Fork the Repository

If you do not have write access to the repository, create a personal copy by clicking the **Fork** button on GitHub.

```text
Original Repository
        │
        ▼
Your Fork
```

This allows you to make changes without affecting the original project.

---

# Clone the Repository

Clone your fork to your local computer.

```bash
git clone https://github.com/your-username/project.git
```

Move into the project directory.

```bash
cd project
```

---

# Create a Branch

Never work directly on the **main** branch.

Create a new branch for each feature or bug fix.

```bash
git switch -c feature/login
```

Examples:

```text
feature/dashboard

bugfix/navbar

docs/readme

hotfix/payment
```

---

# Make Changes

Implement only one logical task per branch.

Examples:

- Fix one bug
- Add one feature
- Improve documentation
- Refactor one module

Keeping branches focused makes reviews easier.

---

# Commit Your Changes

Stage your changes.

```bash
git add .
```

Create a meaningful commit.

```bash
git commit -m "feat: add login page"
```

Good examples:

```text
feat: add search functionality

fix: resolve mobile navigation bug

docs: improve installation guide

refactor: simplify authentication service
```

Avoid:

```text
update

final

test

123
```

---

# Push to GitHub

Upload your branch.

```bash
git push -u origin feature/login
```

---

# Open a Pull Request

Navigate to GitHub and create a Pull Request.

A good Pull Request should include:

- Clear title
- Description of the changes
- Related Issue
- Testing information

Example:

```text
## Changes

- Added login page
- Added form validation
- Updated navigation

Closes #12
```

---

# Code Review

Maintainers review your Pull Request.

They may:

- ✅ Approve
- 💬 Ask questions
- ✏ Request changes

Address review comments before merging.

---

# After Your Pull Request is Merged

Update your local repository.

```bash
git switch main
```

```bash
git pull
```

Delete the completed branch.

```bash
git branch -d feature/login
```

If using your own fork, update it with the latest changes from the original repository before starting new work.

---

# Best Practices

✅ Read the project's README before contributing.

---

✅ Check existing Issues before creating a new one.

---

✅ Create one branch per task.

---

✅ Write meaningful commit messages.

---

✅ Keep Pull Requests small and focused.

---

✅ Follow the project's coding style.

---

✅ Test your changes before submitting.

---

✅ Be respectful during discussions and code reviews.

---

# Common Mistakes

| ❌ Avoid | ✅ Prefer |
|----------|-----------|
| Working directly on `main` | Create a feature branch |
| Large Pull Requests | Small, focused Pull Requests |
| Poor commit messages | Use meaningful commit messages |
| Ignoring project guidelines | Read the documentation first |
| Skipping tests | Verify your changes before submitting |
| Mixing unrelated changes | One task per branch |

---

# Quick Reference

| Step | Action |
|------|--------|
| 1 | Fork Repository |
| 2 | Clone Repository |
| 3 | Create Branch |
| 4 | Make Changes |
| 5 | Commit Changes |
| 6 | Push Branch |
| 7 | Open Pull Request |
| 8 | Review |
| 9 | Merge |

---

# Summary

Contributing is more than writing code—it's about collaborating effectively with others. Following a consistent contribution workflow helps maintain high code quality, simplifies reviews, and creates a positive experience for everyone involved in the project.
