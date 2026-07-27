# Expected Output

## git status

```text
On branch main

nothing to commit, working tree clean
```

---

## Create Branch

```text
Switched to branch 'GitWork'
```

---

## Commit

```text
[GitWork xxxxxx]

Added hello.xml
```

---

## git log

```text
* GitWork

* main
```

---

## git diff

Displays the differences between `main` and `GitWork`.

---

## git merge

```text
Auto-merging hello.xml

CONFLICT (content): Merge conflict in hello.xml

Automatic merge failed.
```

---

## Conflict Markers

```text
<<<<<<< HEAD

<message>Hello from Main Branch</message>

=======

<message>Hello from GitWork</message>

>>>>>>> GitWork
```

---

## After Resolution

```text
[main]

Resolved merge conflict
```

---

## Delete Branch

```text
Deleted branch GitWork.
```

---

## Final Status

```text
On branch main

nothing to commit, working tree clean
```

---

## Result

✔ Merge conflict created

✔ Conflict resolved

✔ Repository synchronized

✔ Branch deleted

✔ Working tree clean