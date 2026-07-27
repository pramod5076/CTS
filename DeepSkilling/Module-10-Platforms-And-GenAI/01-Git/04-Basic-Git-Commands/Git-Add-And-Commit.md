# git add and git commit

## git add

The `git add` command stages changes before committing them.

### Add a Single File

```bash
git add index.html
```

---

### Add Multiple Files

```bash
git add file1.txt file2.txt
```

---

### Add All Files

```bash
git add .
```

---

### Using Wildcards

Add all Markdown files

```bash
git add *.md
```

Add all text files

```bash
git add *.txt
```

---

## git commit

A commit saves the staged changes to the local repository.

### Syntax

```bash
git commit -m "Commit message"
```

### Example

```bash
git commit -m "Added login page"
```

---

## Good Commit Messages

✔ Add user authentication

✔ Fix login validation bug

✔ Update README documentation

Avoid

❌ Changes

❌ Update

❌ Work

---

## Workflow

```
Modify Files
      │
git add
      │
Staging Area
      │
git commit
      │
Local Repository
```

---

## Summary

Use `git add` to stage changes and `git commit` to permanently record those changes with a meaningful message.