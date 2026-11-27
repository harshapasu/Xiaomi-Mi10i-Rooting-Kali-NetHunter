# LineageOS Installation Record

This page documents the installed result, not a universal flashing recipe.

## Recorded result

LineageOS 24.0 is installed on the Xiaomi Mi 10i device target `gauguin`.

## Record these implementation details

- Installation date
- Exact ROM package filename and source
- Package checksum
- Recovery version
- Whether data was backed up
- Any optional Google Apps package and version, if installed
- First boot result
- Post-install verification

## Verify

```bash
adb shell getprop ro.lineage.version
adb shell getprop ro.build.version.release
```

Do not flash a boot/recovery/system image until its target and compatibility with the installed build are verified.
