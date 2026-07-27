# Creating Your Own New Network

Users can create custom Docker networks for better isolation and communication between containers.

## Syntax

```bash
docker network create NETWORK_NAME
```

## Example

```bash
docker network create mynetwork
```

Verify the network:

```bash
docker network ls
```

Run a container using the new network:

```bash
docker run --network mynetwork nginx
```

## Benefits

- Improved container isolation
- Secure communication
- Better organization
- Easier multi-container application management