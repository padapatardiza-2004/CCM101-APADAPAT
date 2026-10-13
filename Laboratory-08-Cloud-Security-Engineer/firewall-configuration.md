# Firewall Configuration

##  SSH Connections

Command used:

```bash
sudo ufw allow ssh
```

This rule permits SSH traffic, allowing administrators to access and manage the server remotely.

## Set Default Firewall Policies

Commands used:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command rejects incoming traffic unless a specific rule permits it. The second command allows outgoing traffic by default.

## Permit Web Application Traffic on Port 8080

Command used:

```bash
sudo ufw allow 8080/tcp
```

This rule permits TCP connections through port 8080, which is used to access the web application.

## SSH Access Consideration

Enabling UFW before adding the necessary SSH rule may interrupt remote administration. When incoming traffic is denied by default, SSH connections can be blocked if they have not been explicitly permitted.
