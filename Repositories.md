# Repositories

A repository (often called a **repo**) is the central place where a project's files, folders, and version history are stored. Every Git project is managed inside a repository.

---

# What is a Repository?

A repository is a storage location that contains:

* Project files
* Source code
* Documentation
* Images and assets
* Commit history
* Branches
* Tags

Think of a repository as the **home of your project**.

---

# Types of Repositories

There are two main types of repositories.

## Local Repository

A local repository exists on your computer.

You can edit files, create commits, and manage branches without an internet connection.

Example:

```text
C:\Projects\MyProject
```

---

## Remote Repository

A remote repository is stored on a hosting platform such as GitHub.

It allows developers to:

* Share code
* Collaborate with teammates
* Back up projects
* Review code
* Manage Issues and Pull Requests

---

# Local vs Remote Repository

| Local Repository        | Remote Repository        |
| ----------------------- | ------------------------ |
| Stored on your computer | Stored online            |
| Works offline           | Requires internet        |
| Used for development    | Used for collaboration   |
| Private by default      | Can be public or private |

---

# Repository Structure

A typical repository may look like this:

```text
my-project/
│
├── README.md
├── LICENSE
├── .gitignore
├── src/
├── images/
├── docs/
└── .git/
```

The hidden `.git` folder contains all Git metadata and version history.

---

# Creating a Repository

You can create a repository in two ways.

## Method 1: Create a New Repository

```bash
git init
```

This initializes Git in the current folder.

---

## Method 2: Clone an Existing Repository

```bash
git clone https://github.com/username/project.git
```

This downloads an existing repository from GitHub.

---

# Repository Lifecycle

```text
Create Repository
        │
        ▼
Write Code
        │
        ▼
Commit Changes
        │
        ▼
Push to GitHub
        │
        ▼
Collaborate
        │
        ▼
Maintain
```

---

# Public and Private Repositories

## Public Repository

Anyone can:

* View the code
* Clone the repository
* Open Issues
* Submit Pull Requests (if permitted)

Examples:

* Open-source projects
* Educational repositories
* Portfolio projects

---

## Private Repository

Only authorized users can access the repository.

Commonly used for:

* Company projects
* Client work
* Personal applications

---

# Important Repository Files

## README.md

Introduces the project and explains how to use it.

---

## LICENSE

Defines how others may use the project.

---

## .gitignore

Specifies files and folders that Git should ignore.

Examples:

```text
node_modules/
.env
venv/
__pycache__/
```

---

# Connecting to GitHub

After creating a local repository, connect it to GitHub.

```bash
git remote add origin https://github.com/username/project.git
```

Check the connection:

```bash
git remote -v
```

---

# Repository Workflow

```text
Local Repository
        │
        ▼
git add
        │
        ▼
git commit
        │
        ▼
git push
        │
        ▼
GitHub Repository
```

---

# Best Practices

* Keep repositories organized.
* Add a clear `README.md`.
* Use a `.gitignore` file.
* Write meaningful commit messages.
* Create branches for new features.
* Archive or delete unused repositories.
* Keep sensitive information out of the repository.

---

# Frequently Used Repository Commands

| Command                 | Description                          |
| ----------------------- | ------------------------------------ |
| `git init`              | Create a new local repository        |
| `git clone`             | Download an existing repository      |
| `git remote -v`         | View connected remote repositories   |
| `git remote add origin` | Connect a local repository to GitHub |
| `git push`              | Upload changes to GitHub             |
| `git pull`              | Download and merge changes           |
| `git fetch`             | Download changes without merging     |

---

# Summary

A repository is the foundation of every Git project. It stores your project's files, version history, branches, and documentation. Local repositories are used for development, while remote repositories on platforms like GitHub enable collaboration, backup, and project management.
