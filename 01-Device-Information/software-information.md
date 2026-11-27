# Software Information

## Recorded software stack

| Layer | Recorded state |
|---|---|
| Android ROM | LineageOS 24.0 |
| Build | `24.0-20261118-NIGHTLY-gauguin` |
| Recovery | Lineage Recovery |
| Root manager | Magisk 31.1 |
| Root access | Working |
| Termux | Configured |
| Kali NetHunter | Rooted setup completed |

Verify current values with:

```bash
adb shell getprop ro.build.version.release
adb shell getprop ro.build.version.security_patch
adb shell getprop ro.lineage.version
adb shell uname -a
```
