# Merging Changes and Merge Conflicts

## What is Merging?

Merging combines changes from one branch into another.

Example

```
main
 │
 ├───────────── feature-login
 │                    │
 └────────────────────┘
        Merge
```

---

## Merge a Branch

Switch to the target branch.

```bash
git checkout main
```

Merge the feature branch.

```bash
git merge feature-login
```

---

## Fast-Forward Merge

Occurs when the target branch has not diverged.

```
main

↓

feature

↓

Merge

↓

Linear History
```

---

## Three-Way Merge

Occurs when both branches have new commits.

Git creates a merge commit to combine the histories.

---

## Merge Conflict

A conflict occurs when the same part of a file has been modified differently in two branches.

Example

Branch A

```text
Welcome Students
```

Branch B

```text
Welcome Developers
```

Git cannot determine which change to keep automatically.

---

## Conflict Markers

```text
<<<<<<< HEAD

Welcome Students

=======

Welcome Developers

>>>>>>> feature-login
```

---

## Resolve Conflict

1. Edit the file.
2. Remove conflict markers.
3. Save the file.
4. Stage the resolved file.

```bash
git add .
```

5. Commit the merge.

```bash
git commit -m "Resolved merge conflict"
```

---

## Best Practices

- Pull latest changes before merging.
- Keep branches short-lived.
- Merge frequently.
- Write meaningful commit messages.
- Test after merging.

---

## Summary

Merging integrates work from multiple branches, while merge conflicts require manual resolution when overlapping changes occur.