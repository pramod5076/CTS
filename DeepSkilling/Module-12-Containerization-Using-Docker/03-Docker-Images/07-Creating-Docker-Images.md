# Creating Docker Images

## Interactive Method

Create a container.

Modify it manually.

Commit the changes.

Example:

```bash
docker commit container_name myimage:v1
```

---

## Dockerfile Method

Create a Dockerfile.

Example:

```dockerfile
FROM ubuntu

RUN apt update

CMD ["bash"]
```

Build the image.

```bash
docker build -t myimage:v1 .
```

The Dockerfile method is the recommended approach because it is repeatable and version-controlled.