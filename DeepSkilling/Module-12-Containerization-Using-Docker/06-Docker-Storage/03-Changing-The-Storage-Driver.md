# Changing the Storage Driver for a Container

The Docker storage driver is configured in the Docker daemon configuration file.

Example:

```json
{
  "storage-driver": "overlay2"
}
```

After updating the configuration, restart Docker.

```bash
sudo systemctl restart docker
```

> **Note:** Changing the storage driver may affect existing images and containers. Always back up important data before making changes.