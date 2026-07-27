# Run a Container and Publish Container Ports

Port publishing allows access to services running inside the container.

## Syntax

```bash
docker run -p HOST_PORT:CONTAINER_PORT IMAGE
```

## Example

```bash
docker run -p 8080:80 nginx
```

In this example:

- Host Port: **8080**
- Container Port: **80**

Access the application using:

```
http://localhost:8080
```