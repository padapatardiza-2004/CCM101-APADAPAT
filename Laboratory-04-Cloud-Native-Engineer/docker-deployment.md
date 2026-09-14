# Docker Deployment

## Checkpoint 3 - Docker Verification

### 1. Check Docker Version

```bash
docker --version
```

This command displays the installed Docker version.

### 2. Check Docker Environment

```bash
docker info
```

This command displays information about the Docker server and its current environment.

## Checkpoint 4 - Nginx Deployment

### 3. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the Nginx image so it can be used to create a container.

### 4. Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and starts an Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

### 5. Test the Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx server through port 8080 and displays the returned HTML.

## Checkpoint 5 - Container Lifecycle

### 6. List Running Containers

```bash
docker ps
```

This command shows the containers that are currently running.

### 7. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 8. Verify the Container Is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### 9. Remove the Container

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container.

### 10. Verify the Container Was Removed

```bash
docker ps -a
```

This command lists all containers so the removal can be verified.
