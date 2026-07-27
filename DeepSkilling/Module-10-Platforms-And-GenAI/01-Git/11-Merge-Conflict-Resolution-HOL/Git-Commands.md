# Git Commands Used

## Repository Status

```bash
git status
```

---

## Create Branch

```bash
git branch GitWork
```

---

## Switch Branch

```bash
git checkout GitWork
```

---

## Create File

```bash
echo "<message>Hello</message>" > hello.xml
```

---

## Stage Changes

```bash
git add .
```

---

## Commit

```bash
git commit -m "Added hello.xml"
```

---

## View Log

```bash
git log --oneline --graph --decorate --all
```

---

## Compare Branches

```bash
git diff main GitWork
```

---

## Visual Comparison

```bash
git difftool main GitWork
```

---

## Merge

```bash
git merge GitWork
```

---

## Resolve Conflict

```bash
git add hello.xml

git commit -m "Resolved merge conflict"
```

---

## Delete Branch

```bash
git branch -d GitWork
```