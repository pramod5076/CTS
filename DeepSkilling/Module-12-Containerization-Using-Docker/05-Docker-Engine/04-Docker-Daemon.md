# Docker Daemon

Docker Daemon (`dockerd`) is the background service responsible for managing Docker objects.

It listens for Docker API requests and performs operations on behalf of the Docker CLI.

## Responsibilities

- Build Docker images
- Run containers
- Stop containers
- Remove containers
- Manage Docker networks
- Manage Docker volumes
- Communicate with container registries

## Workflow

1. User enters a Docker command.
2. Docker CLI sends the request to the Docker Daemon.
3. Docker Daemon performs the requested operation.
4. The result is returned to the Docker CLI.