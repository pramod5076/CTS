# YAML Configuration File

A Docker Compose file is written using YAML syntax.

## Common Sections

- version
- services
- image
- build
- ports
- volumes
- environment
- networks

Example:

```yaml
version: "3.9"

services:
  app:
    image: nginx
    ports:
      - "8080:80"
```

The YAML file defines all containers and their configuration in one place.