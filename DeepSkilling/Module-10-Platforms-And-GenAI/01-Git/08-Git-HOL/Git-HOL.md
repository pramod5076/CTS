# Git Hands-On Lab

## Objective

Learn how to use basic Git commands and work with local and remote repositories.

---

# Step 1

Verify Git Installation

```bash
git --version
```

Expected Output

```text
git version 2.x.x
```

---

# Step 2

Configure Username

```bash
git config --global user.name "Pramod"
```

---

# Step 3

Configure Email

```bash
git config --global user.email "pramod@example.com"
```

---

# Step 4

Verify Configuration

```bash
git config --list
```

---

# Step 5

(Optional)

Configure Notepad++

```bash
git config --global core.editor "notepad++"
```

---

# Step 6

Create Project

```bash
mkdir GitDemo

cd GitDemo
```

---

# Step 7

Initialize Repository

```bash
git init
```

---

# Step 8

Create File

```bash
echo Welcome to Git > welcome.txt
```

---

# Step 9

View File

```bash
type welcome.txt
```

---

# Step 10

Check Status

```bash
git status
```

---

# Step 11

Stage File

```bash
git add welcome.txt
```

---

# Step 12

Commit Changes

```bash
git commit -m "Added welcome file"
```

---

# Step 13

Add Remote Repository

```bash
git remote add origin <repository-url>
```

---

# Step 14

Verify Remote

```bash
git remote -v
```

---

# Step 15

Pull Changes

```bash
git pull origin main
```

---

# Step 16

Push Changes

```bash
git push -u origin main
```

---

## Result

The local repository is synchronized with the remote repository.