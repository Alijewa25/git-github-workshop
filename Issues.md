# Issues

GitHub Issues are used to track tasks, bugs, feature requests, and project discussions. They help individuals and teams organize work, assign responsibilities, and monitor progress.

---

# What is an Issue?

An Issue is a task or discussion created within a GitHub repository.

Issues can be used to:

* Report bugs
* Request new features
* Suggest improvements
* Track project tasks
* Ask questions
* Plan future work

Think of an Issue as a **to-do item** for your project.

---

# Why Use Issues?

Using Issues helps developers:

* Organize project tasks
* Track progress
* Improve team collaboration
* Prioritize work
* Document problems and solutions
* Connect Issues with Pull Requests

---

# Creating an Issue

1. Open your GitHub repository.
2. Select the **Issues** tab.
3. Click **New Issue**.
4. Enter a title.
5. Write a clear description.
6. Add labels, assignees, or milestones (optional).
7. Click **Create**.

---

# Issue Structure

A well-written Issue usually contains the following sections:

```text
Title

Description

Objective

Tasks

Acceptance Criteria
```

---

# Writing a Good Title

A good title should be short, clear, and descriptive.

Good examples:

```text
Add user authentication
Fix login validation
Update README documentation
Improve mobile navigation
```

Avoid titles like:

```text
Fix
Update
Problem
Test
asdf
```

---

# Description

Describe the problem or task clearly.

Example:

```text
Implement a responsive navigation bar for the homepage. The navigation should work correctly on desktop, tablet, and mobile devices.
```

---

# Objective

Explain the expected outcome.

Example:

```text
Create a fully responsive navigation bar that matches the project design and improves user experience.
```

---

# Tasks

Break the work into smaller tasks using checkboxes.

Example:

```markdown
- [ ] Create HTML structure
- [ ] Add CSS styling
- [ ] Implement responsive layout
- [ ] Test on different screen sizes
```

---

# Acceptance Criteria

Acceptance Criteria define when the Issue can be considered complete.

Example:

```text
- Navigation works on all screen sizes.
- Design matches the provided mockup.
- No layout issues remain.
- Code follows project standards.
```

---

# Labels

Labels help categorize Issues.

Common labels include:

| Label            | Purpose                            |
| ---------------- | ---------------------------------- |
| bug              | Reports a problem or error         |
| feature          | New functionality                  |
| enhancement      | Improvement to an existing feature |
| documentation    | Documentation updates              |
| help wanted      | Community assistance needed        |
| good first issue | Suitable for beginners             |

---

# Assignees

An Assignee is the person responsible for completing the Issue.

One or more developers can be assigned to an Issue.

---

# Milestones

Milestones group multiple Issues into a common goal.

Examples:

* Version 1.0
* Version 2.0
* Sprint 1
* Sprint 2

---

# Issue Templates

Many repositories use templates to ensure every Issue contains the required information.

Example template:

```markdown
## Description

Describe the task.

## Objective

What should be achieved?

## Tasks

- [ ] Task 1
- [ ] Task 2
- [ ] Task 3

## Acceptance Criteria

- [ ] Requirement 1
- [ ] Requirement 2
```

---

# Closing an Issue

An Issue can be closed:

* Manually from GitHub
* Automatically through a Pull Request

Example commit message:

```text
Fixes #15
```

or

```text
Closes #15
```

When the Pull Request is merged, GitHub automatically closes the referenced Issue.

---

# Best Practices

* Create one Issue for one task.
* Write clear and descriptive titles.
* Provide enough details in the description.
* Use checklists for larger tasks.
* Assign the Issue to the responsible developer.
* Add appropriate labels.
* Link Issues with Pull Requests whenever possible.
* Close Issues after the work is completed.

---

# Example Issue

```markdown
Title:
Add Login Page

## Description

Create a responsive login page for the application.

## Objective

Allow users to securely log into their accounts.

## Tasks

- [ ] Create login form
- [ ] Add input validation
- [ ] Connect authentication API
- [ ] Test functionality

## Acceptance Criteria

- [ ] Login page is responsive
- [ ] Validation works correctly
- [ ] Authentication is successful
- [ ] Code passes review
```

---

# Workflow

```text
Identify a Task
        │
        ▼
Create an Issue
        │
        ▼
Assign Developer
        │
        ▼
Create a Branch
        │
        ▼
Develop the Feature
        │
        ▼
Commit Changes
        │
        ▼
Push to GitHub
        │
        ▼
Open Pull Request
        │
        ▼
Review
        │
        ▼
Merge
        │
        ▼
Issue Closed
```

---

# Summary

GitHub Issues are an essential project management tool. They help teams organize work, report bugs, request new features, assign responsibilities, and track progress. When combined with branches and Pull Requests, Issues create a structured and efficient development workflow.
