# 02 — Windows Drivers and Tools

## Host environment

- Computer: Lenovo Windows laptop
- Android Platform Tools directory recorded as:

```text
C:\Users\Lenovo\Downloads\platform-tools-latest-windows\platform-tools
```

## Tools

| Tool | Role |
|---|---|
| Android Platform Tools | ADB and Fastboot binaries |
| Android USB driver | Windows-to-device USB communication |
| ADB | Android debugging interface |
| Fastboot | Bootloader communication |
| Git | Repository version control |
| Python | Runtime for selected security tools |

## Verify

Open Command Prompt in the Platform Tools directory:

```bat
adb version
fastboot --version
adb devices
```

For a device in Fastboot mode:

```bat
fastboot devices
```

If ADB reports `unauthorized`, unlock the phone and approve the computer's RSA authorization prompt. Do not publish the device serial number.

## Evidence

Save sanitized ADB/Fastboot screenshots in `../Screenshots/device/`.
