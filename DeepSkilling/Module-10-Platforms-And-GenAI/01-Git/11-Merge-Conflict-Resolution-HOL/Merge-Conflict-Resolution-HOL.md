# Merge Conflict Resolution Hands-On Lab

## Objective

Learn how Git handles merge conflicts and how to resolve them using Git and P4Merge.

---

# Step 1

Verify repository status.

```bash
git status
```

---

# Step 2

Create a new branch.

```bash
git branch GitWork

git checkout GitWork
```

---

# Step 3

Create hello.xml.

```bash
echo "<message>Hello from GitWork</message>" > hello.xml
```

---

# Step 4

Check status.

```bash
git status
```

---

# Step 5

Commit the branch changes.

```bash
git add .

git commit -m "Added hello.xml in GitWork"
```

---

# Step 6

Switch to main.

```bash
git checkout main
```

---

# Step 7

Create another hello.xml with different content.

```bash
echo "<message>Hello from Main Branch</message>" > hello.xml
```

---

# Step 8

Commit changes.

```bash
git add .

git commit -m "Added hello.xml in main"
```

---

# Step 9

View commit history.

```bash
git log --oneline --graph --decorate --all
```

---

# Step 10

Compare branches.

```bash
git diff main GitWork
```

---

# Step 11

(Optional)

Launch P4Merge.

```bash
git difftool main GitWork
```

---

# Step 12

Merge the branch.

```bash
git merge GitWork
```

A merge conflict will occur.

---

# Step 13

Open hello.xml.

Git shows conflict markers.

```text
<<<<<<< HEAD

=======

>>>>>>> GitWork
```

Resolve the conflict manually or using P4Merge.

---

# Step 14

Commit resolved file.

```bash
git add hello.xml

git commit -m "Resolved merge conflict"
```

---

# Step 15

Update .gitignore.

```text
*.bak
```

---

# Step 16

Commit .gitignore.

```bash
git add .gitignore

git commit -m "Updated .gitignore"
```

---

# Step 17

List branches.

```bash
git branch
```

---

# Step 18

Delete merged branch.

```bash
git branch -d GitWork
```

---

# Step 19

View final log.

```bash
git log --oneline --graph --decorate
```

---

## Result

Merge conflict resolved successfully and repository updated.