# 04 — LineageOS

## Recorded installation

- ROM: LineageOS 24.0
- Device target: `gauguin`
- Recorded package: `lineage-24.0-20261118-nightly-gauguin-signed.zip`
- Recovery: Lineage Recovery
- Recorded build property: `24.0-20261118-NIGHTLY-gauguin`
- Extracted image recorded: `boot.img`
- Recorded image size: 128 MiB

## Verify installed build

```bash
adb shell getprop ro.lineage.version
adb shell getprop ro.build.version.release
adb shell getprop ro.build.version.security_patch
```

## Compatibility and safety

Use only ROM packages and images explicitly intended for the exact device target and build. A boot image from another build may be incompatible. Preserve the original and patched images, checksums, and a recovery/backup plan.

This repository records the installed ROM; consult the ROM maintainer's official instructions for current installation and update procedures.
