# Git Commands

This document covers the essential Git commands that every beginner should know. Each command includes its purpose, syntax, and an example.

---

# 1. Check Git Version

Before using Git, verify that it is installed on your computer.

### Command

```bash
git --version
```

### Example

```bash
git --version
```

Output:

```text
git version 2.xx.x
```

---

# 2. Configure Git

Git stores your name and email address. This information appears in every commit you create.

### Set Username

```bash
git config --global user.name "Your Name"
```

### Set Email

```bash
git config --global user.email "your@email.com"
```

### View Configuration

```bash
git config --list
```

---

# 3. Initialize a Repository

Creates a new Git repository in the current directory.

### Command

```bash
git init
```

After running this command, Git creates a hidden `.git` folder that contains the repository history and configuration.

---

# 4. Clone a Repository

Downloads an existing repository from GitHub (or another Git hosting platform) to your computer.

### Command

```bash
git clone <repository-url>
```

### Example

```bash
git clone https://github.com/username/project.git
```

---

# 5. Check Repository Status

Displays the current state of your repository.

### Command

```bash
git status
```

This command shows:

* Modified files
* New files
* Deleted files
* Staged changes
* Untracked files

---

# 6. Add Files to the Staging Area

Before creating a commit, changes must be added to the staging area.

### Add a Single File

```bash
git add filename
```

### Add All Files

```bash
git add .
```

---

# 7. Commit Changes

A commit saves a snapshot of the staged changes.

### Command

```bash
git commit -m "Add login page"
```

Use short and meaningful commit messages.

Examples:

```text
Add navigation bar
Fix login validation
Update README
Remove unused files
```

---

# 8. View Commit History

Displays the repository history.

### Full History

```bash
git log
```

### Short History

```bash
git log --oneline
```

---

# 9. Compare Changes

Shows the differences between the current version and the last commit.

### Command

```bash
git diff
```

To compare staged changes:

```bash
git diff --staged
```

---

# 10. Restore Changes

Discard changes made to a file before committing.

### Command

```bash
git restore filename
```

To remove a file from the staging area without deleting your changes:

```bash
git restore --staged filename
```

---

# 11. Create and Manage Branches

Branches allow developers to work on new features without affecting the main project.

### View Branches

```bash
git branch
```

### Create a Branch

```bash
git branch feature-login
```

### Switch to a Branch

```bash
git switch feature-login
```

### Create and Switch

```bash
git switch -c feature-login
```

---

# 12. Merge Branches

Combines changes from one branch into another.

### Command

```bash
git merge feature-login
```

Merge is usually performed after a feature has been completed.

---

# 13. Connect to a Remote Repository

Links your local repository to GitHub.

### Command

```bash
git remote add origin <repository-url>
```

Example:

```bash
git remote add origin https://github.com/username/project.git
```

View connected remotes:

```bash
git remote -v
```

---

# 14. Push Changes

Uploads local commits to GitHub.

### First Push

```bash
git push -u origin main
```

### Next Pushes

```bash
git push
```

---

# 15. Pull Changes

Downloads and merges the latest changes from the remote repository.

### Command

```bash
git pull
```

---

# 16. Fetch Changes

Downloads updates from the remote repository without merging them.

### Command

```bash
git fetch
```

Unlike `git pull`, this command does not automatically update your current branch.

---

# 17. Temporarily Save Changes

Save unfinished work without creating a commit.

### Save Changes

```bash
git stash
```

### Restore Changes

```bash
git stash pop
```

---

# 18. Create Tags

Tags are commonly used to mark software releases.

### Create a Tag

```bash
git tag v1.0
```

### List Tags

```bash
git tag
```

---

# Git Workflow

The basic Git workflow follows these steps:

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

# Most Frequently Used Commands

| Command             | Description                      |
| ------------------- | -------------------------------- |
| `git init`          | Initialize a new repository      |
| `git clone`         | Download an existing repository  |
| `git status`        | Check repository status          |
| `git add .`         | Stage all changes                |
| `git commit -m ""`  | Create a commit                  |
| `git log --oneline` | View commit history              |
| `git diff`          | Compare changes                  |
| `git branch`        | List branches                    |
| `git switch`        | Switch branches                  |
| `git merge`         | Merge branches                   |
| `git remote -v`     | View remote repositories         |
| `git push`          | Upload changes                   |
| `git pull`          | Download and merge changes       |
| `git fetch`         | Download changes without merging |
| `git stash`         | Temporarily save changes         |
