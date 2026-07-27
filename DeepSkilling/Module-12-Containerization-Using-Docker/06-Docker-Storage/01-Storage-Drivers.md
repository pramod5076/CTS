# Storage Drivers

A Docker storage driver controls how image layers and writable container layers are stored on the host system.

Storage drivers are responsible for managing file systems used by Docker images and containers.

## Common Storage Drivers

- overlay2 (default on most Linux systems)
- aufs
- btrfs
- zfs
- devicemapper

## Advantages

- Efficient image storage
- Layer sharing
- Faster container startup
- Reduced disk usage