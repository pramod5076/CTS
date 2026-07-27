# Data Volumes

Docker volumes provide persistent storage for containers.

Unlike the writable container layer, volumes are stored outside the container lifecycle.

## Benefits

- Persistent data
- Easy backup and restore
- Data sharing between containers
- Better performance
- Independent of container deletion

## Example

```bash
docker run -v myvolume:/app/data nginx
```