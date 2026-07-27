# Git as a Distributed Version Control System (DVCS)

## What is a DVCS?

A Distributed Version Control System allows every developer to have a complete copy of the repository, including the full history of changes.

Unlike centralized systems, developers can work independently without requiring constant access to a central server.

---

## How DVCS Works

```
           Remote Repository
                  │
      ┌───────────┼───────────┐
      ▼           ▼           ▼
 Developer A  Developer B  Developer C
(Local Repo) (Local Repo) (Local Repo)
```

Each developer has:

- Complete project files
- Full commit history
- Ability to commit locally
- Ability to work offline

---

## Advantages

- Offline development
- Faster operations
- Reliable backups
- Better collaboration
- Easy branching and merging

---

## Centralized vs Distributed

| Feature | Centralized VCS | Distributed VCS (Git) |
|----------|-----------------|------------------------|
| Repository | Central Server | Every Developer |
| Offline Work | ❌ | ✅ |
| Full History | Server Only | Local + Remote |
| Speed | Moderate | Fast |
| Backup | Server Dependent | Multiple Copies |

---

## Summary

Git's distributed architecture improves reliability, collaboration, and flexibility, making it the preferred version control system for modern software projects.