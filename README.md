# mountnfs_Linux
mount a network drive in linux to TRUNAS for backup pourposes



in your linux ubunt container
cd /mnt
then
create a foler called backups



cd /etc/sudo nano fstab 
and enter this line and save the fstab

//192.168.0.35/NAS14TBData/SQLNightlyBackups /mnt/backups cifs username=noe,password=duke2929,uid=1000,gid=1000,iocharset=utf8,noperm 0 0

then run sudo mount -a

