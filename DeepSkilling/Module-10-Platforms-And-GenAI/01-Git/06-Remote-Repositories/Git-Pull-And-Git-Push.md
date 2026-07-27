# git pull and git push

## git push

The `git push` command uploads local commits to a remote repository.

### Syntax

```bash
git push origin main
```

Example

```bash
git push origin main
```

---

## First Push

```bash
git push -u origin main
```

The `-u` option sets the upstream branch.

---

## git pull

The `git pull` command downloads changes from a remote repository and merges them into the current branch.

### Syntax

```bash
git pull origin main
```

Example

```bash
git pull origin main
```

---

## Difference

| Command | Purpose |
|----------|---------|
| `git push` | Upload local commits to a remote repository |
| `git pull` | Download and merge changes from a remote repository |

---

## Typical Workflow

```text
Modify Files
      │
git add
      │
git commit
      │
git push
      ▼
Remote Repository
      ▲
git pull
      │
Latest Changes
```

---

## Best Practices

- Pull before pushing to avoid conflicts.
- Commit changes before pushing.
- Review changes after pulling.
- Use meaningful commit messages.

---

## Summary

`git push` uploads your work, while `git pull` keeps your local repository synchronized with the remote repository.