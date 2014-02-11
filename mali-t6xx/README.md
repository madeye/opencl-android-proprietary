## Proprietary OpenCL drivers for ARM's Mali-T6xx GPUs

### 4.3 Jelly Bean

Drivers from Galaxy Note 10.1 2013 edition

```bash
$ adb push jellybean/system/lib /sdcard/
$ adb shell
$ su
# mount -o rw,remount -t yaffs2 /dev/block/mtdblock3 /system
# cp /sdcard/libOpenCL.so /system/lib/
# chmod 644 /system/lib/libOpenCL.so
```
