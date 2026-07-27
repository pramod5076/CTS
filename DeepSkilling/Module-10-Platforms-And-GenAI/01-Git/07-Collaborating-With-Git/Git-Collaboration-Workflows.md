# Git Collaboration Workflows

A Git workflow defines how developers collaborate on a project.

---

# 1. Centralized Workflow

All developers work with a single shared repository.

```
Developer A

        │

Developer B

        │

Developer C

        │

Shared Repository
```

### Advantages

- Simple
- Easy to learn
- Suitable for small teams

---

# 2. Feature Branch Workflow

Each feature is developed in a separate branch.

```
main

 │

 ├── feature-login

 ├── feature-payment

 └── feature-profile
```

### Advantages

- Parallel development
- Safe feature isolation
- Easy code review

---

# 3. Forking Workflow

Each developer forks the repository before contributing.

```
Original Repository

      │

 ├───────────────┐

 ▼               ▼

Fork A         Fork B

 │               │

Pull Request    Pull Request

       │

       ▼

Original Repository
```

### Advantages

- Excellent for open-source projects
- Contributors don't need direct write access
- Improved security

---

# 4. Gitflow Workflow

Gitflow organizes development using dedicated branches.

```
main

 │

 ├── develop

 ├── feature/*

 ├── release/*

 └── hotfix/*
```

### Branch Purpose

- **main** → Production-ready code
- **develop** → Integration branch
- **feature/** → New features
- **release/** → Release preparation
- **hotfix/** → Emergency production fixes

---

## Workflow Comparison

| Workflow | Best For |
|----------|----------|
| Centralized | Small teams |
| Feature Branch | Most software projects |
| Forking | Open-source projects |
| Gitflow | Large enterprise projects |

---

## Summary

Selecting the right workflow depends on project size, team structure, and release strategy.