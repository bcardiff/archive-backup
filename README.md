# archive-backup

This image archives `/target` . The archive is a `.tar.gz` left in `/backup`.

The backup script is based on [tutumcloud/mysql-backup](https://github.com/tutumcloud/mysql-backup).

## Parameters

```
CRON_TIME       the interval of cron job to run mysqldump. `0 0 * * *` by default, which is every day at 00:00
MAX_BACKUPS     the number of backups to keep. When reaching the limit, the old backup will be discarded. No limit by default
INIT_BACKUP     if set, create a backup when the container starts
```
