# Git Ignore Hands-On Lab

## Objective

Learn how to ignore unwanted files and folders using `.gitignore`.

---

# Step 1

Navigate to your Git repository.

```bash
cd GitDemo
```

---

# Step 2

Create a log folder.

```bash
mkdir logs
```

---

# Step 3

Create log files.

```bash
echo Error Log > error.log

echo Application Log > logs/app.log
```

---

# Step 4

Create a `.gitignore` file.

```bash
touch .gitignore
```

Or

```bash
notepad .gitignore
```

---

# Step 5

Add the following rules.

```text
*.log

logs/
```

---

# Step 6

Save the file.

---

# Step 7

Check repository status.

```bash
git status
```

Only the `.gitignore` file should appear.

---

# Step 8

Stage the `.gitignore` file.

```bash
git add .gitignore
```

---

# Step 9

Commit changes.

```bash
git commit -m "Added .gitignore file"
```

---

# Step 10

Push changes.

```bash
git push origin main
```

---

## Result

Git ignores all `.log` files and the `logs` folder.