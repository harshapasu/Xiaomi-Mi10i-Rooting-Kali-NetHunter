# Magisk and Root Troubleshooting

An earlier root check returned an error similar to:

```text
/system/bin/sh: su: inaccessible or not found
```

The project later reached a working root state.

Verification:

```bash
su -c id
```

Record the ROM build, Magisk version, exact output and the actual steps that resolved the issue. Do not flash a boot image unless it is confirmed to match the exact installed ROM build and device target.
