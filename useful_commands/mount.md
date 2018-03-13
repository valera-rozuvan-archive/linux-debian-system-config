sudo fdisk -l

sudo mount -t ext2 /dev/sdb /media/usb

sudo mount -t ntfs -o silent,async,atime,noexec,uid=1000,gid=1000,umask=007 /dev/sdb2 /media/usb
