# Backup Script Guide

## 1. Purpose

This script creates a compressed backup of the `app-data` folder and saves it inside the `backups` directory. It adds a timestamp to each archive filename so backups from different runs can be identified easily.

## 2. Bash Script

```bash
#!/bin/bash
# Backup automation for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Starting the backup process..."

# Make sure the destination folder exists
mkdir -p "$BACKUP_DIR"

# Create a compressed archive of the source folder
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup process finished at $TIMESTAMP."
```

**Note:** The final message appears even if the `tar` command fails. To confirm whether the backup succeeded, check the command output and verify that the archive was created.

## 3. File Permissions

Run the following command to make the script executable:

```bash
chmod +x backup.sh
```

After setting the permission, start the script with:

```bash
./backup.sh
```

The user must have permission to access the script and the folders it uses.

## 4. Cron Schedule

Use this Cron expression to schedule the script to run every day at 2:00 AM:

```cron
0 2 * * * /root/backup.sh
```

The schedule has five fields:

| Field | Value | Description |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The path `/root/backup.sh` must match the actual location of the script. Cron uses the system's configured time zone.

## 5. Verification

Use the following command to list the backup files:

```bash
ls -lh backups/
```

To check the contents of a specific archive, run:

```bash
tar -tzf backups/backup_FILENAME.tar.gz
```

Replace `backup_FILENAME.tar.gz` with the actual archive filename. If the command lists the archived files without an error, the archive can be read and its contents inspected.
