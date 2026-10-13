

## Mission Overview

This laboratory activity focuses on protecting a containerized web application through firewall configuration. It involves running an Nginx container, checking application availability, and applying UFW rules to control incoming network connections.

## Objectives

- Apply the Principle of Least Privilege.
- Examine network exposure from a running web service.
- Set a default policy for incoming connections.
- Permit SSH and TCP port 8080 as required by the lab.
- Verify firewall rules and application accessibility.

## Commands Executed

```bash
docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl -I --max-time 5 http://localhost:8080
```

## Skills Learned

This activity provided practice in running an Nginx container, checking a web service with curl, and managing firewall rules with UFW. It also demonstrated the importance of restricting incoming traffic while permitting the connections required by an application.
