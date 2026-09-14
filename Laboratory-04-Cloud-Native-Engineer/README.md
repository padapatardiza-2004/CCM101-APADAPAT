# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory activity focused on learning the basic concepts of containerization and Docker. I compared virtual machines and containers and then used KillerCoda to deploy an Nginx web server inside a Docker container.

## Objectives

* Differentiate Virtual Machines from containers.
* Use a Docker-enabled Linux environment.
* Execute basic Docker CLI commands.
* Pull and run an Nginx container.
* Test a containerized web server.
* Manage the lifecycle of a Docker container.
* Document the procedures using Markdown.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
docker ps -a
```

## Skills Learned

I learned how to verify a Docker environment, download an image, create and run a container, map a network port, test a web server, and manage the lifecycle of a container. I also practiced organizing technical documentation and screenshots in a GitHub repository.

## Challenges Encountered

One challenge I encountered was understanding how port mapping connects the host machine to a service running inside a container. Running the Nginx container and testing it with curl helped me understand the relationship between the host port and the container port.

