# Mounting disk devices

List available disk devices:

```
sudo fdisk -l
```

Mount device with `ext2` file system:

``` 
sudo mount -t ext2 /dev/sdb /media/usb
```

Mount device with NTFS system:

```
sudo mount -t ntfs -o silent,async,atime,noexec,uid=1000,gid=1000,umask=007 /dev/sdb2 /media/usb
```
