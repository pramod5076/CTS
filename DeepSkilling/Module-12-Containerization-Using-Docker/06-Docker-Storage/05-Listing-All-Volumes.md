# Listing All Volumes

List all Docker volumes using:

```bash
docker volume ls
```

Example Output:

```text
DRIVER    VOLUME NAME

local     myvolume

local     project_data
```

To inspect a volume:

```bash
docker volume inspect myvolume
```