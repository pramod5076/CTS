# Git Components

Git primarily consists of three local components that manage the flow of changes.

---

# 1. Working Directory

The Working Directory contains the files currently being edited by the developer.

Example:

```
Student.java
README.md
index.html
```

Changes made here are **not yet tracked** until staged.

---

# 2. Staging Area (Index)

The Staging Area is an intermediate location where selected changes are prepared before creating a commit.

Purpose:

- Review changes
- Select specific files
- Prepare commit

Command:

```bash
git add filename
```

---

# 3. Local Repository

The Local Repository stores committed snapshots of the project on the developer's machine.

Command:

```bash
git commit -m "Initial commit"
```

---

# Relationship Between Components

```
Edit Files
     │
     ▼
Working Directory
     │
git add
     ▼
Staging Area
     │
git commit
     ▼
Local Repository
     │
git push
     ▼
Remote Repository
```

---

## Common Commands

| Command | Purpose |
|----------|---------|
| `git init` | Initialize a Git repository |
| `git add` | Move changes to the Staging Area |
| `git commit` | Save changes to the Local Repository |
| `git push` | Upload commits to a Remote Repository |
| `git pull` | Download changes from a Remote Repository |

---

## Summary

Understanding the Working Directory, Staging Area, and Repository is essential to mastering the Git workflow and using Git effectively.