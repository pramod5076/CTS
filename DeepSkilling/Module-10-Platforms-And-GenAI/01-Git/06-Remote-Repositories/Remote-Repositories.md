# Adding Remote Repositories

## What is a Remote Repository?

A remote repository is a shared repository stored on a server or cloud platform.

Examples

- GitHub
- GitLab
- Bitbucket
- Azure Repos

---

## View Existing Remotes

```bash
git remote -v
```

Example Output

```text
origin  https://github.com/user/project.git (fetch)
origin  https://github.com/user/project.git (push)
```

---

## Add a Remote Repository

Syntax

```bash
git remote add origin <repository-url>
```

Example

```bash
git remote add origin https://github.com/user/project.git
```

---

## Verify Remote

```bash
git remote -v
```

---

## Remove a Remote

```bash
git remote remove origin
```

---

## Rename a Remote

```bash
git remote rename origin upstream
```

---

## Multiple Remotes

A project can have more than one remote.

Example

```bash
git remote add origin https://github.com/user/project.git

git remote add backup https://github.com/company/project.git
```

View all remotes

```bash
git remote -v
```

---

## Summary

Git supports one or more remote repositories, making collaboration and repository management flexible.