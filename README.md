# mountnfs_Linux

when you have a linux ubuntu container make sure to create it as an unprivileged container is set to NO or you will not be able to mount external drives to it.
![image](https://github.com/user-attachments/assets/434d6f7a-182c-4a05-bb5e-926a3788ea76)

mount a network drive in linux to TRUNAS for backup pourposes



in your linux ubunt container
cd /mnt
then
create a foler called backups



cd /etc/sudo nano fstab 
and enter this line and save the fstab

//192.168.0.35/NAS14TBData/SQLNightlyBackups /mnt/backups cifs username=noe,password=duke2929,uid=1000,gid=1000,iocharset=utf8,noperm 0 0

then run sudo mount -a

