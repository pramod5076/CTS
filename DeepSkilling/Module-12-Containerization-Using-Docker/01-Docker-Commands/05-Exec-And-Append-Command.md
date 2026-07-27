# Exec and Append Command

## Execute a Command Inside a Running Container

```bash
docker exec CONTAINER_ID COMMAND
```

### Example

```bash
docker exec -it mycontainer bash
```

---

## Append a Command During Container Creation

```bash
docker run ubuntu ls
```

The command `ls` runs immediately after the container starts.

### Another Example

```bash
docker run ubuntu echo "Hello Docker"
```

This executes the specified command inside the container.