##Reference
Install rclone.

### Crontab

```
0 2,12,20 * * * rclone sync --copy-links --fast-list --exclude-from /home/martin/.exclude-file.txt /home/martin/docks backblaze:docker-docks 2>&1 >> /home/martin/.logs/rclone.log

15 4,12,20 * * * rclone sync --copy-links --fast-list /home/martin/archive/tier-1 backblaze:tier-1 2>&1 >> /home/martin/.logs/rclone.log
```

