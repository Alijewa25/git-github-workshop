# Merge Conflicts

A merge conflict occurs when Git cannot automatically combine changes from two branches. This usually happens when the same part of a file has been modified in different branches.

Merge conflicts are a normal part of collaborative software development and can be resolved manually.

---

# What is a Merge Conflict?

A merge conflict happens when Git finds conflicting changes and cannot determine which version should be kept.

Git pauses the merge process and asks the developer to resolve the conflict.

---

# Why Do Merge Conflicts Happen?

Merge conflicts commonly occur when:

* Two developers edit the same line of a file.
* One developer deletes a file while another modifies it.
* Changes are made in different branches before they are merged.
* The local branch is outdated compared to the remote branch.

---

# Example Scenario

Suppose two developers are working on the same file.

### Branch: `main`

```text id="3d87c1"
Welcome to our website.
```

### Branch: `feature/homepage`

```text id="sl4m7n"
Welcome to our amazing website.
```

Git cannot automatically decide which version should remain.

---

# Creating a Merge Conflict

Create a feature branch.

```bash id="w9thbc"
git switch -c feature/login
```

Modify a file and commit the changes.

```bash id="l4bw2m"
git add .

git commit -m "Update login page"
```

Switch back to the `main` branch.

```bash id="8r4j0h"
git switch main
```

Modify the same lines in the same file.

Commit again.

```bash id="t6gm3w"
git add .

git commit -m "Update homepage"
```

Merge the feature branch.

```bash id="v7fqsp"
git merge feature/login
```

Git will report a merge conflict if the same lines were modified.

---

# Conflict Markers

Git marks conflicts inside the affected file.

Example:

```text id="mfjlwm"
<<<<<<< HEAD
Welcome to our website.
=======
Welcome to our amazing website.
>>>>>>> feature/login
```

Meaning:

* `<<<<<<< HEAD` → Current branch
* `=======` → Separator
* `>>>>>>> feature/login` → Incoming branch

---

# Resolving a Conflict

Edit the file manually and keep the correct version.

Example:

```text id="8wg8c4"
Welcome to our amazing website.
```

Remove all conflict markers.

---

# Finish the Merge

After resolving the conflict:

```bash id="1sbbj8"
git add .
```

Then create a merge commit.

```bash id="8sd7vt"
git commit
```

Git completes the merge.

---

# Abort a Merge

If you do not want to continue the merge:

```bash id="1afmlo"
git merge --abort
```

This restores the repository to its previous state.

---

# Checking Repository Status

If a conflict occurs:

```bash id="s9vkgt"
git status
```

Git displays which files need attention.

---

# Preventing Merge Conflicts

Although conflicts cannot always be avoided, they can be reduced by following good practices.

* Pull the latest changes before starting new work.
* Merge frequently.
* Keep branches short-lived.
* Communicate with teammates.
* Work on different files whenever possible.
* Commit changes regularly.

---

# Best Practices

* Read the conflict carefully before editing.
* Do not delete code without understanding it.
* Test the project after resolving conflicts.
* Resolve one conflict at a time.
* Commit only after confirming everything works correctly.

---

# Merge Conflict Workflow

```text id="0rjrkj"
Two Branches
      │
      ▼
Modify Same File
      │
      ▼
git merge
      │
      ▼
Merge Conflict
      │
      ▼
Resolve Manually
      │
      ▼
git add .
      │
      ▼
git commit
      │
      ▼
Merge Completed
```

---

# Frequently Used Commands

| Command              | Description                                  |
| -------------------- | -------------------------------------------- |
| `git merge <branch>` | Merge another branch into the current branch |
| `git status`         | Show conflicted files                        |
| `git add .`          | Mark conflicts as resolved                   |
| `git commit`         | Complete the merge                           |
| `git merge --abort`  | Cancel the merge process                     |

---

# Summary

Merge conflicts occur when Git cannot automatically combine changes from different branches. Developers must resolve the conflicting sections manually, stage the resolved files, and complete the merge. Understanding how to resolve merge conflicts is an essential skill for working with Git and collaborating in software development.
