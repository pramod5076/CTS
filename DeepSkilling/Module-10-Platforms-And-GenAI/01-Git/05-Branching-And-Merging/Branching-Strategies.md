# Branching Strategies

A branching strategy defines how branches are created, managed, and merged throughout a project's lifecycle.

---

# 1. Feature Branching

Each new feature is developed in a separate branch.

```
main
 │
 ├──── feature-login
 │
 ├──── feature-payment
 │
 └──── feature-profile
```

### Advantages

- Isolated development
- Easy code review
- Safer integration

---

# 2. Release Branching

A release branch is created when preparing a production release.

```
main
 │
 ├──── release-v1.0
 │
 └──── release-v2.0
```

### Advantages

- Stable releases
- Bug fixes without affecting new development
- Easier testing

---

# 3. Git Flow Workflow

Git Flow uses multiple long-lived and short-lived branches.

```
main
 │
 ├──── develop
 │
 ├──── feature/*
 │
 ├──── release/*
 │
 └──── hotfix/*
```

### Branch Types

- **main** – Production-ready code
- **develop** – Integration branch
- **feature/** – New features
- **release/** – Release preparation
- **hotfix/** – Urgent production fixes

---

## Comparison

| Strategy | Best Use Case |
|-----------|---------------|
| Feature Branching | Developing individual features |
| Release Branching | Preparing production releases |
| Git Flow | Large teams with structured release cycles |

---

## Best Practices

- Use descriptive branch names.
- Delete merged branches.
- Keep branches focused on one task.
- Protect the main branch.
- Review code before merging.

---

## Summary

Choosing the appropriate branching strategy improves collaboration, simplifies releases, and helps maintain a stable codebase.