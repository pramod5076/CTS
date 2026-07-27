# Run a Docker Container and Remove It Once the Process is Complete

The `--rm` option automatically removes the container after it exits.

## Syntax

```bash
docker run --rm IMAGE
```

## Example

```bash
docker run --rm hello-world
```

This option is useful for temporary containers because it avoids leaving unused containers on the system.