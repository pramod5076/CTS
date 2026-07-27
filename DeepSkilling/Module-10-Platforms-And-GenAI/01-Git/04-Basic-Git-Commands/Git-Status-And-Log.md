# git status and git log

## git status

Displays the current state of the repository.

### Syntax

```bash
git status
```

Example Output

```text
On branch main

Changes not staged for commit

Changes to be committed

Untracked files
```

---

## Common File States

- Untracked
- Modified
- Staged
- Committed

---

## git log

Displays the commit history.

### Syntax

```bash
git log
```

---

## Example

```text
commit a8d12f4

Author: Pramod

Date:

Added Login Module
```

---

## Useful Options

### Compact Output

```bash
git log --oneline
```

---

### Last 5 Commits

```bash
git log -5
```

---

### Graph View

```bash
git log --graph
```

---

### Detailed Statistics

```bash
git log --stat
```

---

### One-Line Graph

```bash
git log --oneline --graph
```

---

## Repository Lifecycle

```
Working Directory
        │
git status
        │
git add
        │
git commit
        │
git log
```

---

## Summary

`git status` helps monitor the current repository state, while `git log` provides the complete history of commits with several formatting options for easier analysis.