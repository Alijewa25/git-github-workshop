# Advanced GitHub Features

> This guide introduces additional GitHub features commonly used in professional software development. While these features are not required for every project, understanding them will improve your productivity, collaboration, and repository management.

---

# Table of Contents

- GitHub Actions
- SSH Authentication
- Semantic Versioning
- Repository Templates
- GitHub Pages
- GitHub Discussions
- GitHub Wiki
- GitHub CLI
- Dependabot
- Security Features
- Summary

---

# GitHub Actions

GitHub Actions is GitHub's built-in Continuous Integration and Continuous Deployment (CI/CD) platform.

It automates repetitive development tasks.

## Common Use Cases

| Task | Example |
|------|---------|
| Testing | Run unit tests automatically |
| Build | Build the application |
| Deploy | Deploy to production |
| Linting | Check code quality |
| Notifications | Send deployment alerts |

Workflow location:

```text
.github/workflows/
```

---

# SSH Authentication

SSH provides a secure way to communicate with GitHub without entering your password repeatedly.

## Advantages

- Secure authentication
- Faster than HTTPS
- Recommended for developers
- Supports multiple repositories

Generate a key:

```bash
ssh-keygen -t ed25519
```

Test connection:

```bash
ssh -T git@github.com
```

---

# Semantic Versioning

Semantic Versioning follows the format:

```text
MAJOR.MINOR.PATCH
```

Example:

```text
v2.5.1
```

| Part | Meaning |
|------|----------|
| Major | Breaking changes |
| Minor | New features |
| Patch | Bug fixes |

Examples:

```
1.0.0

↓

1.1.0

↓

1.1.1

↓

2.0.0
```

---

# Repository Templates

GitHub supports reusable templates.

Common templates include:

- Issue Template
- Bug Report
- Feature Request
- Pull Request Template

Templates ensure consistency across projects.

---

# GitHub Pages

GitHub Pages allows developers to host static websites directly from a GitHub repository.

Common uses:

- Portfolio
- Documentation
- Landing Pages
- Project Websites

---

# GitHub Discussions

GitHub Discussions provides a dedicated space for conversations outside of Issues.

Suitable for:

- Questions
- Ideas
- Community support
- Announcements

---

# GitHub Wiki

A Wiki provides project documentation separate from the README.

Typical content:

- User Guide
- API Documentation
- Tutorials
- FAQs

---

# GitHub CLI

GitHub CLI allows developers to interact with GitHub from the terminal.

Examples:

```bash
gh auth login
```

```bash
gh repo create
```

```bash
gh issue create
```

```bash
gh pr create
```

---

# Dependabot

Dependabot automatically checks project dependencies for updates and security vulnerabilities.

Benefits:

- Automatic dependency updates
- Security alerts
- Pull Requests for outdated packages

---

# Security Features

GitHub provides several built-in security tools.

| Feature | Purpose |
|---------|---------|
| Secret Scanning | Detect exposed secrets |
| Dependabot Alerts | Identify vulnerable packages |
| Code Scanning | Analyze code for security issues |
| Branch Protection | Prevent unsafe changes |
| Two-Factor Authentication | Improve account security |

---

# Professional Repository Checklist

A professional GitHub repository should include:

- ✅ README.md
- ✅ LICENSE
- ✅ .gitignore
- ✅ CONTRIBUTING.md
- ✅ GitHub Issues
- ✅ Pull Requests
- ✅ GitHub Projects
- ✅ Labels
- ✅ Releases
- ✅ Semantic Versioning
- ✅ GitHub Actions
- ✅ Branch Protection
- ✅ Repository Documentation

---

# Summary

GitHub offers much more than source code hosting. Features such as GitHub Actions, SSH authentication, Semantic Versioning, GitHub Pages, Discussions, Wiki, CLI, and security tools help teams automate workflows, improve collaboration, strengthen security, and manage projects more effectively. Learning these features prepares developers for professional software development environments.
