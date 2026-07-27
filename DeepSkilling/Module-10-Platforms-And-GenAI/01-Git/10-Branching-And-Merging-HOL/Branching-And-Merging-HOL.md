# Git Branching and Merging Hands-On Lab

## Objective

Learn how to create branches, commit changes, compare branches, merge branches, and delete merged branches.

---

# Step 1

Create a new branch.

```bash
git branch GitNewBranch
```

---

# Step 2

List all local and remote branches.

```bash
git branch -a
```

Observe the `*` symbol indicating the current branch.

---

# Step 3

Switch to the new branch.

```bash
git checkout GitNewBranch
```

Modern Git:

```bash
git switch GitNewBranch
```

---

# Step 4

Create files.

```bash
echo "This file is in new branch" > newfile.txt

mkdir newfolder

echo "Another file" > newfolder/info.txt
```

---

# Step 5

Check repository status.

```bash
git status
```

---

# Step 6

Stage files.

```bash
git add .
```

---

# Step 7

Commit changes.

```bash
git commit -m "Added new files in GitNewBranch"
```

---

# Step 8

Switch back to main.

```bash
git checkout main
```

or

```bash
git checkout master
```

---

# Step 9

Compare branches.

```bash
git diff main GitNewBranch
```

---

# Step 10

(Optional)

Compare visually using P4Merge.

```bash
git difftool main GitNewBranch
```

---

# Step 11

Merge the branch.

```bash
git merge GitNewBranch
```

---

# Step 12

View commit history.

```bash
git log --oneline --graph --decorate
```

---

# Step 13

Delete the merged branch.

```bash
git branch -d GitNewBranch
```

---

# Step 14

Verify status.

```bash
git status
```

---

## Result

The feature branch has been successfully merged into the main branch and deleted.