# git init and git clone

## git init

The `git init` command initializes a new Git repository in the current directory.

### Syntax

```bash
git init
```

### Example

```bash
mkdir StudentPortal

cd StudentPortal

git init
```

Output

```text
Initialized empty Git repository
```

---

## git clone

The `git clone` command creates a complete copy of an existing repository.

### Syntax

```bash
git clone <repository-url>
```

### Example

```bash
git clone https://github.com/user/project.git
```

Git downloads:

- Project files
- Commit history
- Branches
- Configuration

---

## Difference

| git init | git clone |
|----------|-----------|
| Creates a new repository | Copies an existing repository |
| Empty history | Complete history |
| Used for new projects | Used for existing projects |

---

## Workflow

```
New Project
      │
git init
      │
Start Development
```

```
Existing Project
      │
git clone
      │
Start Working
```

---

## Summary

Use `git init` when starting a new project and `git clone` when working with an existing repository.