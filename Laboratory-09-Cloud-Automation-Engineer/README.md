# Mission 9: The Cloud Automation Engineer

## Mission Overview

This mission focuses on automating application data backups using a Bash script and scheduling the task with Linux Cron.

## Objectives

- Understand Bash scripts, variables, and cron jobs.
- Create sample application data.
- Write and execute a backup script.
- Modify file permissions using `chmod`.
- Schedule the backup to run daily at 2:00 AM.
- Document the work and capture screenshots.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Writing Bash scripts.
- Using variables and timestamps.
- Compressing files using `tar`.
- Managing Linux file permissions.
- Scheduling automated tasks with Cron.
- Documenting work in Markdown.
