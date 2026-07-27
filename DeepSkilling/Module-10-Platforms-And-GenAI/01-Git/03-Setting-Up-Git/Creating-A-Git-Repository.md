# Creating a Git Repository

Git repositories can be created in two ways:

1. Initialize a New Repository
2. Clone an Existing Repository

---

# Initialize a New Repository

Navigate to a project folder:

```bash
cd MyProject
```

Initialize Git:

```bash
git init
```

Output

```text
Initialized empty Git repository
```

---

## Check Repository Status

```bash
git status
```

---

## Add Files

```bash
git add .
```

---

## Commit Files

```bash
git commit -m "Initial commit"
```

---

# Clone an Existing Repository

Syntax

```bash
git clone <repository-url>
```

Example

```bash
git clone https://github.com/user/project.git
```

Git downloads the repository and its complete history.

---

## Difference

| Initialize | Clone |
|------------|-------|
| Creates a new empty repository | Copies an existing repository |
| No project history | Includes complete history |
| Used for new projects | Used for existing projects |

---

## Repository Lifecycle

```
Create Folder
      │
      ▼
git init
      │
      ▼
Add Files
      │
      ▼
git add
      │
      ▼
git commit
      │
      ▼
git push
```

---

## Summary

Use `git init` to start a new repository and `git clone` to copy an existing repository. These commands form the foundation of working with Git projects.