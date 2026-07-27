# Run a Container Interactively

Interactive mode allows users to work inside a running container.

## Syntax

```bash
docker run -it IMAGE
```

## Example

```bash
docker run -it ubuntu bash
```

The `-i` option keeps standard input open, and the `-t` option allocates a terminal.