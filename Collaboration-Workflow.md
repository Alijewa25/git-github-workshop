# Collaboration Workflow

> A collaboration workflow defines how developers work together on the same project using Git and GitHub. Following a consistent workflow improves code quality, reduces conflicts, and makes teamwork more efficient.

---

## Table of Contents

- [Why Collaboration Matters](#why-collaboration-matters)
- [Standard Workflow](#standard-workflow)
- [Step-by-Step Process](#step-by-step-process)
- [Example Workflow](#example-workflow)
- [Best Practices](#best-practices)
- [Common Mistakes](#common-mistakes)
- [Quick Reference](#quick-reference)
- [Summary](#summary)

---

# Why Collaboration Matters

Software projects are rarely built by a single developer. Teams often work on multiple features simultaneously.

A structured workflow helps developers:

- Collaborate safely
- Reduce merge conflicts
- Improve code quality
- Track progress
- Maintain a stable main branch

---

# Standard Workflow

```text
Create Issue
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
Approve Changes
      │
      ▼
Merge
      │
      ▼
Delete Branch
```

---

# Step-by-Step Process

## 1. Create an Issue

Before writing code, create an Issue describing the task.

Example:

```
Add user profile page
```

---

## 2. Create a Branch

Never work directly on the **main** branch.

Example:

```bash
git switch -c feature/profile
```

---

## 3. Write Code

Implement only the task assigned to your branch.

Keep changes focused.

---

## 4. Commit Changes

Create small, meaningful commits.

Example:

```bash
git commit -m "feat: add profile page"
```

---

## 5. Push the Branch

Upload your work to GitHub.

```bash
git push -u origin feature/profile
```

---

## 6. Open a Pull Request

Create a Pull Request from your feature branch into **main**.

Include:

- What changed
- Why it changed
- Testing performed
- Linked Issue

Example:

```
Closes #12
```

---

## 7. Code Review

Another developer reviews the Pull Request.

Possible outcomes:

- ✅ Approved
- ✏ Request Changes
- 💬 Discussion

---

## 8. Merge

After approval, merge the Pull Request into the target branch.

Preferred method for most projects:

**Squash and Merge**

---

## 9. Delete the Branch

After merging, remove the feature branch.

```bash
git branch -d feature/profile
```

GitHub also provides a **Delete Branch** button after merging.

---

# Example Workflow

```text
Issue #25
      │
      ▼
feature/profile
      │
      ▼
Code Development
      │
      ▼
Commit
      │
      ▼
Push
      │
      ▼
Pull Request
      │
      ▼
Review
      │
      ▼
Merge
      │
      ▼
Done ✅
```

---

# Best Practices

✅ Create one branch for one task.

---

✅ Keep Pull Requests small.

---

✅ Write meaningful commit messages.

---

✅ Review code before merging.

---

✅ Delete merged branches.

---

✅ Keep the **main** branch stable.

---

# Common Mistakes

| ❌ Avoid | ✅ Prefer |
|----------|-----------|
| Working directly on `main` | Create a feature branch |
| Huge Pull Requests | Small, focused Pull Requests |
| Skipping code reviews | Review every Pull Request |
| One branch for multiple tasks | One branch per feature or bug |
| Forgetting to pull latest changes | Run `git pull` before starting work |

---

# Quick Reference

| Step | Action |
|------|--------|
| 1 | Create Issue |
| 2 | Create Branch |
| 3 | Write Code |
| 4 | Commit Changes |
| 5 | Push Branch |
| 6 | Open Pull Request |
| 7 | Review |
| 8 | Merge |
| 9 | Delete Branch |

---

# Summary

A consistent collaboration workflow is essential for successful software development. By following a structured process—from creating an Issue to merging a reviewed Pull Request—teams can build software more efficiently, reduce errors, and maintain a clean, organized repository.
