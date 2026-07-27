# Create the Compose File

Docker Compose uses a file named:

```text
docker-compose.yml
```

Example:

```yaml
version: "3.9"

services:
  web:
    image: nginx
    ports:
      - "8080:80"
```

Start the application:

```bash
docker compose up
```