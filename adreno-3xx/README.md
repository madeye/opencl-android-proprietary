## Proprietary OpenCL drivers for Qualcomm's Adreno 3xx GPUs

### 4.4 Kitkat

Drivers from
https://developer.qualcomm.com/download/adreno200-hammerhead-kot49h.zip

```bash
$ adb push kitkat/system/vendor/lib /sdcard/
$ adb shell
$ su
# mount -o rw,remount -t yaffs2 /dev/block/mtdblock3 /system
# cp /sdcard/libOpenCL.so /system/vendor/lib/
# cp /sdcard/libllvm-a3xx.so /system/vendor/lib/
# chmod 644 /system/vendor/lib/libOpenCL.so
# chmod 644 /system/vendor/lib/libllvm-a3xx.so
```

### 4.2 Jelly Bean

Drivers from
https://developer.qualcomm.com/download/Adreno200-AU_LINUX_ANDROID_JB_VANILLA_04.02.02.060.053.zip

```bash
$ adb push jellybean/system/lib /sdcard/
$ adb shell
$ su
# mount -o rw,remount -t yaffs2 /dev/block/mtdblock3 /system
# cp /sdcard/libOpenCL.so /system/lib/
# cp /sdcard/libllvm-a3xx.so /system/lib/
# chmod 644 /system/lib/libOpenCL.so
# chmod 644 /system/lib/libllvm-a3xx.so
```
