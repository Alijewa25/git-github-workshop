# Pull Requests

A Pull Request (PR) is a GitHub feature that allows developers to propose changes before merging them into the main branch. It enables code review, discussion, and collaboration.

---

# What is a Pull Request?

A Pull Request is a request to merge changes from one branch into another.

Instead of merging code directly into the `main` branch, developers first create a Pull Request so their teammates can review the changes.

---

# Why Use Pull Requests?

Pull Requests help teams:

* Review code before merging
* Detect bugs early
* Improve code quality
* Encourage collaboration
* Keep project history organized
* Discuss implementation details

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
Approve Changes
        │
        ▼
Merge
        │
        ▼
Delete Branch
```

---

# Creating a Pull Request

1. Push your branch to GitHub.
2. Open your repository.
3. Click **Compare & Pull Request**.
4. Select the correct base and compare branches.
5. Enter a title.
6. Write a description.
7. Request reviewers (optional).
8. Click **Create Pull Request**.

---

# Pull Request Title

The title should clearly describe the changes.

Good examples:

```text
Add login page
Fix responsive navigation
Update README documentation
Refactor authentication module
```

Avoid titles like:

```text
Update
Fix
Test
Final
```

---

# Pull Request Description

A good Pull Request description explains:

* What was changed
* Why it was changed
* Any important notes for reviewers

Example:

```markdown
## Summary

Implemented a responsive login page.

## Changes

- Added login form
- Added input validation
- Improved mobile responsiveness

## Testing

- Tested on desktop
- Tested on mobile devices
```

---

# Code Review

A reviewer examines the Pull Request before it is merged.

The reviewer checks:

* Code quality
* Readability
* Functionality
* Project standards
* Possible bugs

---

# Review Actions

A reviewer can:

* Approve
* Request Changes
* Leave Comments

---

# Merge Options

GitHub provides several merge methods.

### Create a Merge Commit

Preserves all commits and creates a merge commit.

Recommended for beginners.

---

### Squash and Merge

Combines all commits into one before merging.

Useful when a branch contains many small commits.

---

### Rebase and Merge

Applies commits without creating a merge commit.

Creates a cleaner history but is recommended for experienced developers.

---

# Closing Related Issues

A Pull Request can automatically close an Issue.

Example:

```text
Closes #12
```

or

```text
Fixes #12
```

When the Pull Request is merged, GitHub automatically closes the referenced Issue.

---

# Best Practices

* Create one Pull Request for one task.
* Keep Pull Requests small and focused.
* Write clear titles and descriptions.
* Review your own code before submitting.
* Respond to review comments.
* Merge only after approval.
* Delete merged branches.

---

# Example Pull Request

```markdown
Title:
Add User Authentication

## Summary

Implemented user authentication using JWT.

## Changes

- Added login endpoint
- Added registration endpoint
- Added password hashing
- Updated documentation

## Testing

- Login tested
- Registration tested
- Token validation tested
```

---

# Pull Request Lifecycle

```text
Issue Created
      │
      ▼
Branch Created
      │
      ▼
Development
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
Approve
      │
      ▼
Merge
      │
      ▼
Branch Deleted
```

---

# Summary

Pull Requests are an essential part of collaborative software development. They provide a structured way to review code, discuss changes, maintain quality, and safely merge new features into the main branch.
