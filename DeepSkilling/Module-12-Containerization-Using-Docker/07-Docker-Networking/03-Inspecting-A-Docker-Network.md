# Inspecting a Docker Network

Docker provides detailed information about a network using the `inspect` command.

## Syntax

```bash
docker network inspect NETWORK_NAME
```

## Example

```bash
docker network inspect bridge
```

The output includes:

- Network ID
- Driver
- IP subnet
- Gateway
- Connected containers
- Configuration details