# Expected Output

## Folder Structure

```text
GitDemo
│
├── .git
├── .gitignore
├── welcome.txt
├── error.log
└── logs
    └── app.log
```

---

## git status

```text
On branch main

Untracked files:

.gitignore

nothing added to commit but untracked files present
```

Notice that:

- `error.log` is ignored.
- `logs/` directory is ignored.
- Only `.gitignore` appears.

---

## Commit

```text
[main a1b2c3d]

Added .gitignore file

1 file changed
```

---

## Push

```text
Enumerating objects...

Counting objects...

Writing objects...

To https://github.com/username/GitDemo.git
```

---

## Result

✔ `.log` files ignored

✔ `logs/` folder ignored

✔ Working directory is clean

✔ Repository updated successfully