# Xiaomi-Mi10i-Rooting-Kali-NetHunter
Complete Android customization and mobile cybersecurity setup on Xiaomi Mi 10i (M2007J17I). Includes bootloader unlocking, LineageOS 24.0 installation, Magisk root, Termux configuration, and Kali NetHunter setup with mobile security tools.
# Xiaomi Mi 10i — Android Rooting, Customization & Mobile Security

![Device](https://img.shields.io/badge/Device-Xiaomi%20Mi%2010i-blue)
![ROM](https://img.shields.io/badge/ROM-LineageOS%2024.0-blue)
![Root](https://img.shields.io/badge/Root-Magisk%2031.1-brightgreen)
![Architecture](https://img.shields.io/badge/Architecture-ARM64-informational)
![Project](https://img.shields.io/badge/Project-Technical%20Showcase-orange)

A technical repository documenting the completed Android customization and rooted mobile Linux setup on the **Xiaomi Mi 10i (M2007J17I)**. It records device information, Windows ADB/Fastboot setup, bootloader status, LineageOS, Magisk root, Termux, Kali NetHunter, mobile security tooling, verification commands, and troubleshooting.

> **Documentation standard:** confirmed project facts are identified as recorded status. Hardware values, kernel details, exact NetHunter edition, and application versions should be populated from the device's current output rather than guessed.

## Project status

| Area | Recorded status |
|---|---|
| Device | Xiaomi Mi 10i (M2007J17I) |
| Device codename | `gauguininpro` |
| Board codename | `gauguin` |
| Architecture | ARM64 / `aarch64` |
| Bootloader | Unlocked |
| Custom ROM | LineageOS 24.0 installed |
| Recovery | Lineage Recovery |
| Magisk | Version 31.1 installed |
| Root access | Successfully established |
| Termux | Configured |
| Kali NetHunter | Rooted setup and compatibility work completed |
| Host computer | Lenovo Windows laptop |

## Device and software specifications

| Component | Recorded value |
|---|---|
| Model | Xiaomi Mi 10i |
| Model number | M2007J17I |
| Device codename | `gauguininpro` |
| Board codename | `gauguin` |
| Processor platform | Qualcomm |
| CPU architecture | ARM64 / aarch64 |
| ROM | LineageOS 24.0 |
| Recorded build | `24.0-20261118-NIGHTLY-gauguin` |
| Recorded Android version | 17 — verify with current device output |
| Recorded security patch | 1 November 2026 — verify with current device output |
| Recovery | Lineage Recovery |
| Magisk application | 31.1 |
| Zygisk | Disabled in last recorded configuration |
| Root | Working |

The exact RAM, storage, chipset SKU, kernel release, firmware/baseband, and current security patch should be added from the phone's current system information. Do not infer these from the marketing name or an older screenshot.

## Repository contents

| Directory | Contents |
|---|---|
| `01-Device-Information/` | Device identity and system specification commands |
| `02-Drivers-and-Tools/` | Windows drivers, Platform Tools, ADB and Fastboot |
| `03-Bootloader-Unlocking/` | Unlock status and verification |
| `04-LineageOS/` | ROM build, recovery and installation record |
| `05-Magisk-Root/` | Magisk configuration and root verification |
| `06-Root-Applications/` | Root app inventory and permission notes |
| `07-Termux/` | Package setup, shell and Python/Git environment |
| `08-Kali-NetHunter/` | NetHunter environment, root integration and verification |
| `09-Mobile-Security-Tools/` | MobSF, JADX, Burp Suite, ZAP and Wireshark |
| `10-Troubleshooting/` | Recorded errors, diagnosis and outcomes |
| `Screenshots/` | Evidence grouped by implementation stage |

## Key verification commands

Run these from Windows Command Prompt or PowerShell where appropriate:

```bat
adb version
adb devices
fastboot --version
fastboot devices
```

Check device properties:

```bash
adb shell getprop ro.product.model
adb shell getprop ro.product.device
adb shell getprop ro.build.version.release
adb shell getprop ro.build.version.security_patch
adb shell getprop ro.lineage.version
adb shell uname -m
```

Check bootloader state while the device is in Fastboot mode:

```bash
fastboot getvar unlocked
```

Check root from an authorized device shell:

```bash
su -c id
```

A successful root check should return a root identity such as `uid=0(root)`. Exact output can vary by environment.

## Technical notes

- Installing the Magisk APK alone does not prove that root is active; verify with a root command.
- NetHunter CLI availability does not, by itself, prove that every NetHunter feature or external wireless adapter is supported.
- Kernel-dependent features must be checked against the exact device kernel and NetHunter edition.
- Keep a copy of the exact ROM build and matching boot-related images used for this device.
- Do not flash images intended for a different device, codename, or build.

## Security and responsible testing

This repository is for education and authorized security research. Test only devices, applications, networks, and systems that you own or have explicit permission to assess. Use lab applications and test accounts. Do not publish passwords, tokens, private keys, IMEI, phone numbers, account details, or unredacted device identifiers.

## Evidence

Add screenshots to the relevant folders under `Screenshots/`. Hide serial numbers and personal information before committing images.

## Author

**Harsha Vardhan**  
Cybersecurity Enthusiast | VAPT Learner | Android Customization | Linux

**Learn • Experiment • Document • Secure**
