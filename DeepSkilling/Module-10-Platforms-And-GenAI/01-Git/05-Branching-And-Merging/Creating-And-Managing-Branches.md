# Creating and Managing Branches

## What is a Branch?

A branch is an independent line of development in Git. Each branch has its own commits and can be merged into another branch later.

---

## View Branches

```bash
git branch
```

---

## Create a New Branch

```bash
git branch feature-login
```

---

## Switch to a Branch

```bash
git checkout feature-login
```

---

## Create and Switch in One Command

```bash
git checkout -b feature-login
```

---

## Using Modern Git

```bash
git switch feature-login
```

Create and switch:

```bash
git switch -c feature-login
```

---

## List All Branches

```bash
git branch
```

Example

```text
* main
  feature-login
  feature-dashboard
```

The `*` indicates the current branch.

---

## Rename a Branch

```bash
git branch -m old-name new-name
```

---

## Delete a Branch

```bash
git branch -d feature-login
```

Force delete

```bash
git branch -D feature-login
```

---

## Summary

Git branches allow developers to isolate changes, making development safer and more organized.