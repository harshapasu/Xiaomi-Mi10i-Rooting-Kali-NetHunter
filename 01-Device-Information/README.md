# 01 — Device Information

## Device identity

| Property | Recorded value |
|---|---|
| Manufacturer | Xiaomi |
| Device | Mi 10i |
| Model | M2007J17I |
| Device codename | `gauguininpro` |
| Board codename | `gauguin` |
| Platform | Qualcomm |
| Architecture | ARM64 / `aarch64` |

## Software identity

| Property | Recorded value |
|---|---|
| ROM | LineageOS 24.0 |
| Recorded build | `24.0-20261118-NIGHTLY-gauguin` |
| Recovery | Lineage Recovery |
| Magisk | 31.1 |
| Bootloader | Unlocked |
| Root | Working |

Android release, security patch, RAM, storage, kernel, baseband and firmware are intentionally not hardcoded here unless verified from the current device.

## Collect current properties

From the computer:

```bash
adb shell getprop ro.product.manufacturer
adb shell getprop ro.product.model
adb shell getprop ro.product.device
adb shell getprop ro.product.board
adb shell getprop ro.board.platform
adb shell getprop ro.build.version.release
adb shell getprop ro.build.version.security_patch
adb shell getprop ro.lineage.version
adb shell uname -a
adb shell uname -m
adb shell cat /proc/meminfo
adb shell df -h /data
```

Record the date and save sanitized output in `system-information.md`. Storage figures can vary depending on installed apps and user data.

## Evidence

Place sanitized screenshots in `../Screenshots/device/`.
