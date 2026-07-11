# Markdown

Markdown is a lightweight markup language used to format text. GitHub uses Markdown for README files, Issues, Pull Requests, Wikis, Discussions, and documentation.

Markdown is easy to read, easy to write, and does not require special software.

---

# Why Use Markdown?

Markdown allows developers to:

* Create well-structured documentation
* Format text quickly
* Add code blocks
* Create tables
* Insert images and links
* Write professional README files
* Improve project documentation

---

# Headings

Use the `#` symbol to create headings.

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

Output:

# Heading 1

## Heading 2

### Heading 3

---

# Bold and Italic Text

Bold text:

```markdown
**Bold Text**
```

Italic text:

```markdown
*Italic Text*
```

Bold and italic:

```markdown
***Bold and Italic***
```

---

# Strikethrough

```markdown
~~Deleted Text~~
```

Output:

~~Deleted Text~~

---

# Lists

## Unordered List

```markdown
- Apple
- Banana
- Orange
```

Output:

* Apple
* Banana
* Orange

---

## Ordered List

```markdown
1. Install Git
2. Create Repository
3. Push Changes
```

Output:

1. Install Git
2. Create Repository
3. Push Changes

---

# Task Lists

GitHub supports checklists.

```markdown
- [ ] Create README
- [ ] Add documentation
- [x] Create repository
```

Output:

* [ ] Create README
* [ ] Add documentation
* [x] Create repository

---

# Links

Create hyperlinks using the following syntax.

```markdown
[GitHub](https://github.com)
```

Output:

GitHub

---

# Images

Insert images using:

```markdown
![Logo](images/logo.png)
```

---

# Inline Code

Use backticks.

```markdown
Use `git status` to check repository status.
```

Output:

Use `git status` to check repository status.

---

# Code Blocks

Use three backticks.

Example:

````markdown
```bash
git status
git add .
git commit -m "Initial commit"
```
````

Output:

```bash
git status
git add .
git commit -m "Initial commit"
```

---

# Quotes

Create blockquotes using `>`.

```markdown
> Git is a distributed version control system.
```

Output:

> Git is a distributed version control system.

---

# Horizontal Lines

Use three hyphens.

```markdown
---
```

Output:

---

---

# Tables

Markdown supports tables.

```markdown
| Command | Description |
|----------|-------------|
| git init | Create a repository |
| git add . | Stage all changes |
| git commit | Save changes |
```

Output:

| Command    | Description         |
| ---------- | ------------------- |
| git init   | Create a repository |
| git add .  | Stage all changes   |
| git commit | Save changes        |

---

# Emojis

GitHub supports emoji shortcodes.

```markdown
:rocket:
:white_check_mark:
:bug:
:books:
:fire:
```

Common examples:

🚀 📚 🐛 ✅ 🔥

---

# Escaping Characters

Use a backslash (`\`) to display Markdown characters as plain text.

Example:

```markdown
\# This is not a heading
```

Output:

# This is not a heading

---

# Example README

````markdown
# Git Workshop

## Description

Learn the fundamentals of Git and GitHub.

## Topics

- Git Basics
- GitHub
- Branches
- Pull Requests

## Installation

```bash
git clone https://github.com/username/project.git
````

## License

MIT License

``````

---

# Best Practices

- Use headings to organize content.
- Keep paragraphs short.
- Use code blocks for commands.
- Add tables when comparing information.
- Use task lists for progress tracking.
- Keep formatting consistent.
- Write clear and concise documentation.

---

# Most Common Markdown Syntax

| Syntax | Purpose |
|--------|---------|
| `#` | Heading |
| `**text**` | Bold |
| `*text*` | Italic |
| `~~text~~` | Strikethrough |
| `-` | Unordered list |
| `1.` | Ordered list |
| `- [ ]` | Task list |
| `` `code` `` | Inline code |
| ````` ``` ````` | Code block |
| `>` | Quote |
| `---` | Horizontal line |
| `|` | Table |
| `[]()` | Link |
| `![]()` | Image |

---

# Summary

Markdown is the standard formatting language used across GitHub. It makes documentation easier to write and read while providing simple syntax for headings, lists, tables, code blocks, images, and links. Learning Markdown is essential for creating professional README files, Issues, Pull Requests, and project documentation.
``````
