backitup
========

bash script for making snapshots via rsync + rotation of the snapshots (automatically by cron)

written by: robbytobby on 25.6.2012

usage:
just call the script in the crontab:
backitup [ -f CONFIG-FILE ]
if -f is not present it defaults to "backitup.cfg"

see backitup.cfg for options

The script makes rsync-snapshots and rotates them.
It is possible to check the backup-destination for a minimum amount of disk-space.
It is possible to remount the backup-disk ro after the backup runs - this only works
if the backup-base-dir is the mountpoint of the backup-volume. 
