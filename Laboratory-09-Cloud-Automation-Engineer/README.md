# Laboratory 09: Cloud Automation Engineer

## Mission Overview

This laboratory activity introduces task automation in a Linux environment using Bash scripting and Cron. The main task is to create a script that generates compressed backups of application data and schedule it to run automatically.

## Objectives

- Understand the use of automation in cloud operations.
- Create a Bash script for backing up files.
- Set the correct execution permissions.
- Generate and verify backup archives.
- Configure a recurring task using Cron.
- Document the results of the automation process.

## Commands Executed

```bash
mkdir -p app-data
echo "CloudNova backup test" > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -lh backups/
env EDITOR=nano crontab -e
crontab -l
```

## Skills Learned

This activity provided practice in writing Bash scripts, managing file permissions, creating compressed archives, and scheduling recurring tasks with Cron. It also highlighted the importance of checking the generated backups and verifying the scheduled job.
