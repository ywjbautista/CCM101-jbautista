# Backup Script Guide

## 1. Backup Script

The following Bash script creates a timestamped compressed archive of the `app-data` directory.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

mkdir -p $BACKUP_DIR
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The command `chmod +x backup.sh` grants permission to execute the script as a program. This allows it to be run using `./backup.sh`.

## 3. Cron Schedule

```text
0 2 * * * /root/backup.sh
```

The five time fields mean:

- **Minute (`0`):** Runs at minute zero.
- **Hour (`2`):** Runs at 2 AM.
- **Day of Month (`*`):** Runs every day of the month.
- **Month (`*`):** Runs every month.
- **Day of Week (`*`):** Runs every day of the week.

This schedule is intended to run the backup script daily at 2:00 AM.
