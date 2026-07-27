# Configuring Git

After installation, configure your identity so Git can record the author of each commit.

---

## Configure Username

```bash
git config --global user.name "Your Name"
```

Example

```bash
git config --global user.name "Pramod"
```

---

## Configure Email

```bash
git config --global user.email "yourname@example.com"
```

Example

```bash
git config --global user.email "pramod@gmail.com"
```

---

## View Configuration

```bash
git config --list
```

Example Output

```text
user.name=Pramod
user.email=pramod@gmail.com
```

---

## Check Individual Settings

Username

```bash
git config user.name
```

Email

```bash
git config user.email
```

---

## Global vs Local Configuration

| Configuration | Scope |
|--------------|-------|
| Global | All repositories on the system |
| Local | Current repository only |

Local configuration example:

```bash
git config user.name "Developer"
git config user.email "developer@example.com"
```

---

## Summary

Git configuration stores your identity, ensuring every commit records the correct author information.