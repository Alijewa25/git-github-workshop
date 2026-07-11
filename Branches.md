# Branches

Branches are one of Git's most powerful features. They allow developers to work on different tasks independently without affecting the main project.

---

# What is a Branch?

A branch is an independent line of development in a Git repository.

Instead of making changes directly on the `main` branch, developers create a separate branch for each feature, bug fix, or improvement.

This keeps the project organized and prevents unfinished work from affecting the stable version.

---

# Why Use Branches?

Branches help developers:

* Develop new features safely
* Fix bugs without affecting the main branch
* Work on multiple tasks simultaneously
* Collaborate with team members
* Test new ideas without risking the project
* Keep the project history organized

---

# Default Branch

Every Git repository starts with a default branch.

Most modern repositories use:

```text
main
```

Older repositories may use:

```text
master
```

The `main` branch should always contain a stable and working version of the project.

---

# Branch Workflow

```text
             main
              │
      ┌───────┴────────┐
      │                │
      ▼                ▼
feature/login   feature/dashboard
      │                │
      ▼                ▼
     Merge          Merge
      │                │
      └───────┬────────┘
              ▼
             main
```

---

# View Existing Branches

Display all local branches.

```bash
git branch
```

The current branch is marked with an asterisk (`*`).

Example:

```text
* main
  feature/login
  feature/navbar
```

---

# Create a Branch

Create a new branch without switching to it.

```bash
git branch feature/login
```

---

# Switch Branches

Move from one branch to another.

```bash
git switch feature/login
```

Older Git versions use:

```bash
git checkout feature/login
```

---

# Create and Switch

Create a new branch and switch to it immediately.

```bash
git switch -c feature/login
```

or

```bash
git checkout -b feature/login
```

---

# Make Changes

After switching branches, you can edit files, add new features, or fix bugs.

Check the repository status:

```bash
git status
```

---

# Commit Changes

Save your work on the current branch.

```bash
git add .

git commit -m "Add login page"
```

Commits belong only to the current branch until they are merged.

---

# Merge a Branch

After finishing your work, switch back to `main` and merge the branch.

```bash
git switch main
```

```bash
git merge feature/login
```

The changes from `feature/login` are now part of the `main` branch.

---

# Delete a Branch

After merging, the branch is usually no longer needed.

Delete a merged branch:

```bash
git branch -d feature/login
```

Force delete a branch:

```bash
git branch -D feature/login
```

---

# Branch Naming Convention

Use meaningful branch names.

Good examples:

```text
feature/login
feature/user-profile
feature/search-bar

bugfix/login-error
bugfix/navbar

hotfix/payment-crash

docs/readme-update

refactor/database

chore/dependencies
```

Avoid:

```text
test

new

branch1

mybranch

login2
```

---

# Common Branch Prefixes

| Prefix      | Purpose                                     |
| ----------- | ------------------------------------------- |
| `feature/`  | New functionality                           |
| `bugfix/`   | Bug fixes                                   |
| `hotfix/`   | Urgent production fixes                     |
| `docs/`     | Documentation updates                       |
| `refactor/` | Code improvements without changing behavior |
| `chore/`    | Maintenance tasks                           |
| `test/`     | Testing-related work                        |

---

# Merge Conflicts

Sometimes two branches modify the same part of a file.

Git cannot decide which version is correct, resulting in a **merge conflict**.

Example:

```text
Branch A
Hello World

Branch B
Hello GitHub
```

Git asks the developer to resolve the conflict manually before completing the merge.

---

# Best Practices

* Never develop directly on the `main` branch.
* Create one branch for one task.
* Use descriptive branch names.
* Commit frequently.
* Merge completed work as soon as possible.
* Delete branches after merging.
* Keep your branch updated with the latest `main` branch.

---

# Example Workflow

```text
1. Create a Branch
        │
        ▼
2. Make Changes
        │
        ▼
3. git add .
        │
        ▼
4. git commit
        │
        ▼
5. git push
        │
        ▼
6. Open Pull Request
        │
        ▼
7. Review
        │
        ▼
8. Merge
        │
        ▼
9. Delete Branch
```

---

# Frequently Used Branch Commands

| Command                  | Description                            |
| ------------------------ | -------------------------------------- |
| `git branch`             | List local branches                    |
| `git branch <name>`      | Create a new branch                    |
| `git switch <name>`      | Switch to a branch                     |
| `git switch -c <name>`   | Create and switch to a new branch      |
| `git checkout <name>`    | Switch branch (older command)          |
| `git checkout -b <name>` | Create and switch (older command)      |
| `git merge <branch>`     | Merge a branch into the current branch |
| `git branch -d <name>`   | Delete a merged branch                 |
| `git branch -D <name>`   | Force delete a branch                  |

---

# Summary

Branches allow developers to work independently without affecting the stable version of a project. By creating separate branches for features, bug fixes, and improvements, teams can collaborate efficiently, review code safely, and keep the `main` branch stable and production-ready.
