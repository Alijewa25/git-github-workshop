# Git Cheat Sheet

This cheat sheet provides a quick reference for the most commonly used Git commands. Keep it nearby while working on Git projects.

---

# Repository

## Initialize a Repository

```bash
git init
```

Create a new Git repository.

---

## Clone a Repository

```bash
git clone <repository-url>
```

Download an existing repository.

Example:

```bash
git clone https://github.com/username/project.git
```

---

# Configuration

## Set Username

```bash
git config --global user.name "Your Name"
```

---

## Set Email

```bash
git config --global user.email "your@email.com"
```

---

## View Configuration

```bash
git config --list
```

---

# Checking Status

## Repository Status

```bash
git status
```

View modified, staged, and untracked files.

---

## Commit History

```bash
git log
```

---

## Short Commit History

```bash
git log --oneline
```

---

## Compare Changes

```bash
git diff
```

---

# Staging

## Stage One File

```bash
git add filename
```

---

## Stage All Files

```bash
git add .
```

---

# Commits

## Create a Commit

```bash
git commit -m "Commit message"
```

---

## Amend the Last Commit

```bash
git commit --amend
```

Modify the most recent commit.

---

# Branches

## List Branches

```bash
git branch
```

---

## Create a Branch

```bash
git branch feature/login
```

---

## Switch Branches

```bash
git switch feature/login
```

---

## Create and Switch

```bash
git switch -c feature/login
```

---

## Delete a Branch

```bash
git branch -d feature/login
```

---

# Merging

## Merge a Branch

```bash
git merge feature/login
```

---

## Abort a Merge

```bash
git merge --abort
```

---

# Remote Repositories

## View Remote Repositories

```bash
git remote -v
```

---

## Connect to GitHub

```bash
git remote add origin <repository-url>
```

---

# Push & Pull

## Push Changes

```bash
git push
```

---

## First Push

```bash
git push -u origin main
```

---

## Pull Changes

```bash
git pull
```

---

## Fetch Changes

```bash
git fetch
```

---

# Restore

## Restore File

```bash
git restore filename
```

---

## Unstage File

```bash
git restore --staged filename
```

---

# Stash

## Save Changes

```bash
git stash
```

---

## Restore Changes

```bash
git stash pop
```

---

# Tags

## Create a Tag

```bash
git tag v1.0
```

---

## List Tags

```bash
git tag
```

---

# Undo Changes

## Reset to Previous Commit

```bash
git reset --hard HEAD~1
```

Move back one commit and discard changes.

---

## Revert a Commit

```bash
git revert <commit-hash>
```

Undo a commit safely by creating a new commit.

---

# Daily Workflow

```text
git pull

↓

git switch -c feature/new-feature

↓

Write Code

↓

git add .

↓

git commit -m "Add new feature"

↓

git push -u origin feature/new-feature

↓

Open Pull Request

↓

Review

↓

Merge

↓

git switch main

↓

git pull

↓

git branch -d feature/new-feature
```

---

# Most Common Commands

| Command             | Purpose                             |
| ------------------- | ----------------------------------- |
| `git init`          | Create a repository                 |
| `git clone`         | Clone a repository                  |
| `git status`        | Check repository status             |
| `git add .`         | Stage all changes                   |
| `git commit -m`     | Create a commit                     |
| `git log --oneline` | View commit history                 |
| `git diff`          | Compare changes                     |
| `git branch`        | List branches                       |
| `git switch`        | Switch branches                     |
| `git merge`         | Merge branches                      |
| `git push`          | Upload changes                      |
| `git pull`          | Download and merge changes          |
| `git fetch`         | Download changes                    |
| `git stash`         | Save work temporarily               |
| `git restore`       | Restore files                       |
| `git reset`         | Move repository to an earlier state |
| `git revert`        | Safely undo a commit                |
| `git tag`           | Create release tags                 |

---

# Git Workflow at a Glance

```text
Working Directory
        │
        ▼
     git add
        │
        ▼
   Staging Area
        │
        ▼
   git commit
        │
        ▼
 Local Repository
        │
        ▼
    git push
        │
        ▼
 GitHub Repository
```

---

# Summary

This cheat sheet is a quick reference to the essential Git commands used in everyday development. While it does not replace detailed documentation, it serves as a practical guide for common Git workflows and commands.
