# GitHub Pull Requests

> A Pull Request (PR) is a request to merge changes from one branch into another. It enables code review, discussion, automated testing, and collaboration before changes become part of the main codebase.

---

## Table of Contents

- [What is a Pull Request?](#what-is-a-pull-request)
- [Why Use Pull Requests?](#why-use-pull-requests)
- [Pull Request Workflow](#pull-request-workflow)
- [Creating a Pull Request](#creating-a-pull-request)
- [Pull Request Components](#pull-request-components)
- [Review Process](#review-process)
- [Merge Methods](#merge-methods)
- [Draft Pull Requests](#draft-pull-requests)
- [Linking Issues](#linking-issues)
- [Best Practices](#best-practices)
- [Common Mistakes](#common-mistakes)
- [Quick Reference](#quick-reference)
- [Summary](#summary)

---

# What is a Pull Request?

A Pull Request (PR) is a request to merge changes from one branch into another, usually into the **main** branch.

Instead of pushing code directly to the main branch, developers submit a Pull Request so teammates can review the changes before they are merged.

---

# Why Use Pull Requests?

| Benefit | Description |
|----------|-------------|
| 👀 Code Review | Other developers review your code before merging |
| 💬 Team Discussion | Discuss improvements and ask questions |
| 🐞 Bug Detection | Find issues before they reach production |
| 🤝 Collaboration | Multiple developers can work safely together |
| 🤖 Automation | Run tests and checks automatically with GitHub Actions |

---

# Pull Request Workflow

```text
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
Request Changes / Approve
      │
      ▼
Merge
      │
      ▼
Delete Branch
```

---

# Creating a Pull Request

Navigate to:

```text
Repository
    ↓
Pull Requests
    ↓
New Pull Request
```

Choose:

- Base Branch (usually `main`)
- Compare Branch (your feature branch)

Example:

| Base | Compare |
|------|----------|
| main | feature/login |

---

# Pull Request Components

A good Pull Request should contain:

| Component | Purpose |
|-----------|---------|
| Title | Short description of the changes |
| Description | Explain what was changed and why |
| Commits | Related commits |
| Reviewers | Team members reviewing the code |
| Labels | Categorize the PR |
| Linked Issues | Connect related Issues |

---

# Example Pull Request

## Title

```text
Add user authentication system
```

## Description

```text
## Changes

- Added login page
- Added registration page
- Connected authentication API
- Added form validation

## Testing

- Login tested
- Registration tested
- Password validation verified

Closes #15
```

---

# Review Process

A typical Pull Request review follows these steps.

```text
Open Pull Request
        │
        ▼
Code Review
        │
        ▼
Approve
or
Request Changes
        │
        ▼
Developer Updates Code
        │
        ▼
Approve
        │
        ▼
Merge
```

---

# What Reviewers Check

| Review Area | Description |
|-------------|-------------|
| ✅ Functionality | Does the code work correctly? |
| 📖 Readability | Is the code easy to understand? |
| 🎯 Naming | Are variables and functions well named? |
| 🔒 Security | Are there any security risks? |
| ⚡ Performance | Can the implementation be improved? |
| 🧪 Testing | Has the code been tested? |
| 📚 Documentation | Is documentation updated if needed? |

---

# Merge Methods

GitHub provides three merge strategies.

## Merge Commit

Preserves the complete branch history.

```text
feature/login
        │
        ▼
Merge Commit
        │
        ▼
main
```

Best for preserving development history.

---

## Squash and Merge

Combines all commits into a single commit.

Example:

```
5 commits

↓

1 commit
```

Best for keeping a clean Git history.

---

## Rebase and Merge

Replays commits on top of the target branch without creating a merge commit.

Produces a linear project history.

---

# Draft Pull Requests

A Draft Pull Request indicates that the work is still in progress.

Use Draft PRs when:

- Development is incomplete
- Feedback is needed early
- The code is not ready to merge

Draft PRs cannot be merged until they are marked as **Ready for Review**.

---

# Linking Issues

A Pull Request can automatically close related Issues.

Example:

```text
Closes #24
```

Other supported keywords:

```text
Fixes #24
```

```text
Resolves #24
```

Once the Pull Request is merged, GitHub automatically closes the linked Issue.

---

# Best Practices

✅ Create one Pull Request for one feature.

---

✅ Keep Pull Requests small.

Smaller Pull Requests are easier to review.

---

✅ Write clear titles.

Good:

```
Add password reset feature
```

Avoid:

```
Update project
```

---

✅ Provide a detailed description.

Explain:

- What changed
- Why it changed
- How it was tested

---

✅ Request code reviews before merging.

---

✅ Resolve all review comments.

---

✅ Delete merged branches.

This keeps the repository clean.

---

# Common Mistakes

| ❌ Avoid | ✅ Prefer |
|----------|-----------|
| Huge Pull Requests | Small focused Pull Requests |
| Poor descriptions | Explain the changes clearly |
| Skipping reviews | Always request a review |
| Merging broken code | Test before merging |
| Keeping old branches | Delete merged branches |

---

# Quick Reference

| Action | Purpose |
|---------|---------|
| New Pull Request | Request to merge code |
| Review | Inspect code quality |
| Approve | Accept the changes |
| Request Changes | Ask for improvements |
| Merge | Combine branches |
| Close | Reject or cancel the Pull Request |
| Draft | Work in progress |

---

# Summary

Pull Requests are one of GitHub's most important collaboration features. They enable teams to review code, discuss improvements, automate testing, and safely merge changes into the main branch. Following Pull Request best practices leads to cleaner code, better teamwork, and a more maintainable project.
