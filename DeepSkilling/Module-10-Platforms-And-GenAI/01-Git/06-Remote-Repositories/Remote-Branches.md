# Handling Remote Branches

## What are Remote Branches?

Remote branches are branches that exist in a remote repository and represent the work shared by other developers.

---

## View Remote Branches

```bash
git branch -r
```

Example

```text
origin/main

origin/develop

origin/feature-login
```

---

## View Local and Remote Branches

```bash
git branch -a
```

---

## Create a Local Branch from a Remote Branch

```bash
git checkout -b feature-login origin/feature-login
```

Modern Git

```bash
git switch -c feature-login origin/feature-login
```

---

## Push a New Branch

```bash
git push -u origin feature-login
```

---

## Track an Existing Remote Branch

```bash
git branch --track feature-login origin/feature-login
```

---

## Delete a Remote Branch

```bash
git push origin --delete feature-login
```

---

## Remote Branch Workflow

```text
Create Branch
      │
Commit Changes
      │
git push -u origin feature-login
      │
Remote Branch Created
      │
Other Developers
      │
git pull
```

---

## Best Practices

- Use descriptive branch names.
- Delete unused remote branches.
- Keep branches synchronized regularly.
- Pull the latest changes before creating new work.
- Track remote branches correctly.

---

## Summary

Remote branches make collaboration easier by allowing developers to share, track, and synchronize feature development across a team.