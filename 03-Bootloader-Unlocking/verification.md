# Bootloader Verification

With the phone in Fastboot mode:

```bash
fastboot devices
fastboot getvar unlocked
```

Recorded result:

```text
unlocked: yes
```

Capture the result with the serial number hidden and store it in `../../Screenshots/bootloader/`.
