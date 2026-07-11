# Git Flow

Git Flow is a branching strategy that helps developers organize their work and collaborate efficiently. Instead of making changes directly on the `main` branch, each task is developed in a separate branch.

---

# Why Use Git Flow?

Git Flow helps teams:

* Work on multiple features simultaneously
* Prevent accidental changes to the main branch
* Keep the project history organized
* Review code before merging
* Reduce merge conflicts

---

# Git Flow Workflow

```text
          Create Repository
                  │
                  ▼
             Clone Repository
                  │
                  ▼
            Create a Branch
                  │
                  ▼
             Make Changes
                  │
                  ▼
               git add .
                  │
                  ▼
       git commit -m "Message"
                  │
                  ▼
      git push origin branch-name
                  │
                  ▼
        Open Pull Request (PR)
                  │
                  ▼
            Code Review
                  │
                  ▼
          Approve Changes
                  │
                  ▼
         Merge into main
                  │
                  ▼
          Delete Branch
```

---

# Step 1 – Clone the Repository

Download the project from GitHub.

```bash
git clone https://github.com/username/project.git
```

---

# Step 2 – Create a New Branch

Every new feature or bug fix should have its own branch.

```bash
git switch -c feature/login
```

Examples:

```text
feature/login
feature/dashboard
bugfix/navbar
docs/readme
```

---

# Step 3 – Make Changes

Develop the new feature or fix the issue.

Check the repository status:

```bash
git status
```

---

# Step 4 – Stage Changes

Add modified files to the staging area.

```bash
git add .
```

---

# Step 5 – Commit Changes

Save a snapshot of your work.

```bash
git commit -m "Add login page"
```

Use meaningful commit messages.

---

# Step 6 – Push the Branch

Upload your branch to GitHub.

```bash
git push -u origin feature/login
```

---

# Step 7 – Open a Pull Request

Create a Pull Request on GitHub.

A Pull Request allows teammates to:

* Review the code
* Suggest improvements
* Approve changes
* Discuss the implementation

---

# Step 8 – Merge

After the Pull Request is approved, merge the branch into `main`.

```text
feature/login
        │
        ▼
      main
```

---

# Step 9 – Delete the Branch

After merging, delete the branch because its work is complete.

```bash
git branch -d feature/login
```

---

# Best Practices

* Never work directly on the `main` branch.
* Create one branch for one task.
* Commit frequently with meaningful messages.
* Push changes regularly.
* Open Pull Requests for every completed task.
* Review code before merging.
* Delete merged branches.

---

# Summary

```text
Clone Repository
        │
        ▼
Create Branch
        │
        ▼
Write Code
        │
        ▼
git add .
        │
        ▼
git commit
        │
        ▼
git push
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
Delete Branch
```

Git Flow provides a simple and organized workflow that makes collaboration easier, keeps the project stable, and improves code quality.
