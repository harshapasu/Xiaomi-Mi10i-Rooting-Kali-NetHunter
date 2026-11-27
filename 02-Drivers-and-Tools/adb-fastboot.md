# ADB and Fastboot Reference

## ADB checks

```bat
adb version
adb devices
adb shell
```

## Useful device queries

```bash
getprop ro.product.model
getprop ro.product.device
getprop ro.build.version.release
getprop ro.lineage.version
uname -a
```

## Fastboot checks

```bat
fastboot --version
fastboot devices
fastboot getvar unlocked
```

Fastboot commands must be run only when the phone is in the appropriate bootloader/fastboot interface. Do not run flashing or erase commands unless the exact image, partition, device codename and build compatibility have been independently confirmed.
