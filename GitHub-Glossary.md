# GitHub Glossary

> A quick reference guide to the most common Git and GitHub terms every developer should know.

---

## Table of Contents

- [Repository](#repository)
- [Local Repository](#local-repository)
- [Remote Repository](#remote-repository)
- [Git](#git)
- [GitHub](#github)
- [Commit](#commit)
- [Branch](#branch)
- [Main Branch](#main-branch)
- [Clone](#clone)
- [Fork](#fork)
- [Origin](#origin)
- [Upstream](#upstream)
- [Push](#push)
- [Pull](#pull)
- [Fetch](#fetch)
- [Merge](#merge)
- [Merge Conflict](#merge-conflict)
- [Pull Request](#pull-request)
- [Working Directory](#working-directory)
- [Staging Area](#staging-area)
- [HEAD](#head)
- [Tag](#tag)
- [Release](#release)
- [.gitignore](#gitignore)
- [README.md](#readmemd)
- [LICENSE](#license)
- [Issue](#issue)
- [GitHub Actions](#github-actions)
- [Workflow](#workflow)
- [Artifact](#artifact)
- [Summary](#summary)

---

# Repository

A **repository** (or **repo**) is a storage location for a project's source code, files, documentation, and version history.

Example:

```
portfolio/
│
├── README.md
├── src/
├── images/
└── .gitignore
```

---

# Local Repository

A repository stored on your own computer.

You make changes here before sharing them with others.

---

# Remote Repository

A repository hosted on a remote server such as GitHub.

It allows multiple developers to collaborate on the same project.

---

# Git

Git is a distributed Version Control System (VCS) used to track file changes, manage versions, and collaborate with other developers.

---

# GitHub

GitHub is a cloud-based platform that hosts Git repositories and provides collaboration tools such as:

- Pull Requests
- Issues
- GitHub Actions
- Releases
- Discussions
- Project Boards

---

# Commit

A commit is a snapshot of your project at a specific point in time.

Example:

```bash
git commit -m "Add login page"
```

Each commit has its own unique ID (SHA).

---

# Branch

A branch is an independent line of development.

Different features and bug fixes are usually developed in separate branches.

Example:

```
main
│
├── feature/login
├── feature/dashboard
└── bugfix/navbar
```

---

# Main Branch

The default branch of a repository.

It should always contain stable and production-ready code.

---

# Clone

Creates a copy of an existing remote repository on your computer.

Command:

```bash
git clone https://github.com/username/project.git
```

---

# Fork

A personal copy of someone else's GitHub repository.

Forking allows you to experiment without affecting the original project.

---

# Origin

The default name of the remote repository.

Example:

```text
origin → https://github.com/username/project.git
```

---

# Upstream

The original repository from which a fork was created.

Useful when contributing to open-source projects.

---

# Push

Uploads your local commits to a remote repository.

Command:

```bash
git push
```

---

# Pull

Downloads and merges changes from a remote repository.

Command:

```bash
git pull
```

---

# Fetch

Downloads new commits from the remote repository without merging them.

Command:

```bash
git fetch
```

---

# Merge

Combines changes from one branch into another.

Command:

```bash
git merge feature/login
```

---

# Merge Conflict

Occurs when Git cannot automatically combine changes because two versions modify the same lines.

Developers must manually resolve the conflict before continuing.

---

# Pull Request

A Pull Request (PR) is a request to merge one branch into another.

Benefits:

- Code Review
- Team Discussion
- Automated Testing
- Higher Code Quality

---

# Working Directory

The files currently being edited on your computer.

Changes made here are not yet tracked until staged.

---

# Staging Area

A temporary area where changes are prepared before creating a commit.

Command:

```bash
git add .
```

---

# HEAD

HEAD is a pointer to the currently checked-out commit or branch.

It represents your current working position in Git history.

---

# Tag

A tag marks a specific commit, usually representing a release.

Example:

```bash
git tag v1.0.0
```

---

# Release

A release is a published version of a project.

Releases are commonly associated with Git tags and contain release notes.

---

# .gitignore

A configuration file that tells Git which files and directories should not be tracked.

Common examples:

```text
node_modules/
.env
dist/
.vscode/
```

---

# README.md

The main documentation file of a repository.

A professional README usually includes:

- Project Overview
- Installation
- Usage
- Features
- License
- Contribution Guide

---

# LICENSE

Defines how others may use, modify, and distribute your project.

Popular licenses include:

| License | Description |
|----------|-------------|
| MIT | Very permissive |
| Apache 2.0 | Includes patent protection |
| GPL | Requires derivative works to remain open-source |
| BSD | Simple permissive license |

---

# Issue

An Issue is used to report:

- Bugs
- Feature Requests
- Improvements
- Tasks

Issues help organize project development.

---

# GitHub Actions

GitHub Actions is GitHub's built-in Continuous Integration and Continuous Deployment (CI/CD) platform.

It automates tasks such as:

- Running Tests
- Building Projects
- Deployments
- Code Quality Checks

---

# Workflow

A workflow is an automated process executed by GitHub Actions.

Workflows are stored inside:

```text
.github/workflows/
```

---

# Artifact

An artifact is a file generated during a workflow.

Examples include:

- Build files
- Test reports
- Coverage reports
- Deployment packages

---

# Quick Reference

| Term | Meaning |
|------|---------|
| Repository | Project storage |
| Commit | Snapshot of changes |
| Branch | Independent development line |
| Clone | Download repository |
| Fork | Personal copy of another repository |
| Push | Upload commits |
| Pull | Download and merge changes |
| Fetch | Download changes only |
| Merge | Combine branches |
| Pull Request | Request to merge code |
| HEAD | Current Git position |
| Tag | Mark a version |
| Release | Published project version |
| Issue | Track bugs and tasks |
| GitHub Actions | Automation platform |

---

# Summary

Understanding Git and GitHub terminology is essential for effective collaboration and professional software development. Familiarity with these concepts helps developers communicate clearly, navigate repositories confidently, and follow industry-standard workflows.
