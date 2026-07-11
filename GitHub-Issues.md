# GitHub Issues

> GitHub Issues is a built-in project management tool that helps developers track bugs, plan new features, organize tasks, and collaborate efficiently throughout the software development process.

---

## Table of Contents

- [What are GitHub Issues?](#what-are-github-issues)
- [Why Use GitHub Issues?](#why-use-github-issues)
- [Creating an Issue](#creating-an-issue)
- [Issue Types](#issue-types)
- [Issue Components](#issue-components)
- [Issue Lifecycle](#issue-lifecycle)
- [Assigning Issues](#assigning-issues)
- [Closing Issues Automatically](#closing-issues-automatically)
- [Best Practices](#best-practices)
- [Common Mistakes](#common-mistakes)
- [Quick Reference](#quick-reference)
- [Summary](#summary)

---

# What are GitHub Issues?

GitHub Issues are used to plan, organize, discuss, and track work within a repository.

An Issue can represent:

- A bug
- A new feature
- A task
- Documentation updates
- Performance improvements
- Questions
- Ideas

Think of an Issue as a task that needs attention.

---

# Why Use GitHub Issues?

| Benefit | Description |
|----------|-------------|
| 📋 Task Management | Organize development work |
| 🐞 Bug Tracking | Report and fix software issues |
| 💬 Team Discussion | Collaborate directly inside the Issue |
| 📈 Progress Tracking | Monitor project progress |
| 🔗 Integration | Connect Issues with Pull Requests and Projects |

---

# Creating an Issue

Navigate to:

```
Repository
    ↓
Issues
    ↓
New Issue
```

Provide:

- A clear title
- A detailed description
- Labels
- Assignee
- Milestone (optional)

---

# Issue Types

| Type | Description |
|------|-------------|
| 🐞 Bug | Something is not working correctly |
| ✨ Feature | Request a new feature |
| 📚 Documentation | Improve project documentation |
| ⚡ Enhancement | Improve an existing feature |
| ❓ Question | Ask for clarification |
| 🛠 Task | General development work |

---

# Issue Components

A professional Issue usually contains:

| Component | Purpose |
|-----------|---------|
| Title | Short summary |
| Description | Explain the problem or request |
| Labels | Categorize the Issue |
| Assignee | Person responsible |
| Milestone | Related project goal |
| Comments | Discussion and updates |

---

# Example Issue

## Title

```text
Add Dark Mode Support
```

## Description

```text
Implement a dark theme for the application.

Requirements:

- Toggle button
- Save user preference
- Support all pages
```

---

# Issue Lifecycle

```text
Open
   │
   ▼
Assigned
   │
   ▼
In Progress
   │
   ▼
Review
   │
   ▼
Closed
```

Every Issue follows a lifecycle until it is completed.

---

# Assigning Issues

Issues can be assigned to one or more contributors.

Benefits:

- Clear ownership
- Better accountability
- Easier project management

---

# Closing Issues Automatically

GitHub can automatically close an Issue when a Pull Request is merged.

Example:

```text
Closes #15
```

Other supported keywords include:

```text
Fixes #15
```

```text
Resolves #15
```

When the Pull Request is merged, the Issue is closed automatically.

---

# Best Practices

✅ Use clear and descriptive titles.

Example:

```
Fix login validation error
```

Instead of:

```
Bug
```

---

✅ One Issue should represent one task.

---

✅ Provide enough information for others to reproduce the problem.

---

✅ Use Labels.

---

✅ Assign the Issue to the responsible developer.

---

✅ Close Issues after completing the work.

---

# Common Mistakes

| ❌ Avoid | ✅ Prefer |
|----------|-----------|
| Vague titles | Specific titles |
| Multiple tasks in one Issue | One task per Issue |
| No description | Detailed explanation |
| No labels | Categorize every Issue |
| Leaving Issues open forever | Close completed Issues |

---

# Quick Reference

| Action | Purpose |
|---------|---------|
| New Issue | Create a task |
| Assign | Choose responsible developer |
| Label | Categorize Issue |
| Comment | Discuss progress |
| Link PR | Connect development work |
| Close | Mark completed |

---

# Summary

GitHub Issues provide a structured way to manage software development tasks. They improve collaboration, organize project planning, simplify bug tracking, and integrate seamlessly with Pull Requests, Projects, and Milestones.
