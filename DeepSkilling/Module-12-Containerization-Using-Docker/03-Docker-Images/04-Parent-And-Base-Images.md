# Parent Image

A parent image is an existing Docker image used as the starting point for creating a new image.

Example:

```dockerfile
FROM ubuntu:22.04
```

---

# Base Image

A base image is the first image in a Docker build and does not depend on any other image.

Example:

```dockerfile
FROM scratch
```