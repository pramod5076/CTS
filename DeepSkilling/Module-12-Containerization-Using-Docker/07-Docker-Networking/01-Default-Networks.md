# Default Networks

When Docker is installed, it automatically creates three default networks.

## 1. Bridge Network

- Default network for standalone containers.
- Containers on the same bridge network can communicate with each other.

Example:

```bash
docker run -d nginx
```

---

## 2. Host Network

- Shares the host machine's network stack.
- No network isolation between the container and the host.

Example:

```bash
docker run --network host nginx
```

---

## 3. None Network

- Disables networking for the container.
- The container has no external or internal network access.

Example:

```bash
docker run --network none nginx
```