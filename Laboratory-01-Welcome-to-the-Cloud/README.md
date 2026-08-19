# Mission 1 – Welcome to the Cloud

## Mission Overview

This activity introduces the basics of cloud computing using **KillerCoda**. It focuses on Linux commands, file management, system information, and GitHub documentation.

## Objectives

- Use a Linux cloud environment.
- Learn basic Linux commands.
- Manage files and directories.
- Check system information.
- Create a GitHub repository.
- Document activities using Markdown.

# Checkpoint 1 – Entering the Cloud

For this checkpoint, I accessed the Ubuntu Linux environment using KillerCoda. I created a new Linux user account named apadapat, set up its Bash shell and home directory, and granted it sudo privileges. I also used basic Linux commands to verify my username, current directory, and hostname.

### User Information

| Information | Result |
|---|---|
| Current Username | apadapat |
| Current Working Directory | /home/apadapat |
| Hostname | [Your Hostname] |

### Commands Used

```bash
sudo adduser apadapat
sudo usermod -aG sudo apadapat
su - apadapat

whoami
pwd
hostname
