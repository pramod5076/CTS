# Docker Build Context

The Docker build context is the set of files and directories available during the image build process.

When running:

```bash
docker build .
```

Docker sends the current directory to the Docker daemon.

## Best Practices

- Keep the build context small.
- Exclude unnecessary files using `.dockerignore`.
- Store only required application files.