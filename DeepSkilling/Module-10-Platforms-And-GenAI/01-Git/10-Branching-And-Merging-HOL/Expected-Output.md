# Expected Output

## Create Branch

```text
Branch 'GitNewBranch' created successfully.
```

---

## List Branches

```text
* main
  GitNewBranch
```

---

## Switch Branch

```text
Switched to branch 'GitNewBranch'
```

---

## git status

```text
On branch GitNewBranch

Untracked files:

newfile.txt

newfolder/
```

---

## Commit

```text
[GitNewBranch abc1234]

Added new files in GitNewBranch
```

---

## git diff

```text
Shows differences between the main branch and GitNewBranch.
```

---

## git merge

```text
Updating xxxxxx..yyyyyy

Fast-forward

newfile.txt

newfolder/info.txt
```

---

## git log

```text
* abc1234 (HEAD -> main)

Added new files in GitNewBranch

* 89abcd1

Initial Commit
```

---

## Delete Branch

```text
Deleted branch GitNewBranch.
```

---

## Final git status

```text
On branch main

nothing to commit, working tree clean
```

---

## Result

✔ Branch created successfully

✔ Files committed successfully

✔ Branch merged into main

✔ Commit history verified

✔ Branch deleted

✔ Repository is clean