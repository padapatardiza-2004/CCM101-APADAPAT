# Mission Overview

This laboratory activity focuses on the role of a Cloud Operations Engineer. The task involves checking the health of a Linux server, deploying an Nginx web server through Docker, creating test web requests, checking application logs, and observing container resource usage.

# Objectives

- Utilize native Linux command-line tools to monitor host CPU, Memory, and Disk capacity.
- Deploy a web container and track its real-time performance using Docker metrics.
- Generate web traffic and extract application access logs for analysis.
- Translate raw performance data into a readable technical report using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio.

# Monitoring Commands Executed

```bash
free -h
```

```bash
df -h /
```

```bash
top
```

```bash
docker run -d -p 8080:80 --name client-website nginx
```

```bash
curl http://localhost:8080
```

```bash
curl http://localhost:8080/hidden-admin-page
```

```bash
docker logs client-website
```

```bash
docker stats
```

# Skills Learned

- Linux resource monitoring
- Docker container deployment
- Web traffic testing
- Application log checking
- Container performance monitoring
- Basic cloud operations
- Markdown documentation
