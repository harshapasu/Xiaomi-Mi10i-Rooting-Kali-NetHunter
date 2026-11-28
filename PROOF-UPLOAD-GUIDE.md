# Proofs, Screenshots and Command Outputs

Use this guide to add evidence for work you have actually completed. The repository separates visual evidence from text-based command results:

- `Screenshots/` — screenshots or photos showing device screens, app status, and terminal sessions.
- `Outputs/` — plain-text command results, version information, logs, and verification notes.

## What to collect

| Area | Screenshot suggestions | Output suggestions |
|---|---|---|
| Device | About phone, model, Android version | `device-information.txt` |
| Bootloader | Fastboot screen and unlock-status screen | `bootloader-status.txt` |
| LineageOS | About phone, LineageOS version/build, recovery | `lineageos-version.txt` |
| Magisk | Magisk app status and version | `magisk-version.txt` |
| Root | Terminal showing successful root check | `root-verification.txt` |
| Termux | Termux terminal and installed environment | `termux-environment.txt`, `python-version.txt`, `git-version.txt` |
| NetHunter | NetHunter terminal and Kali release information | `nethunter-version.txt`, `kali-release.txt`, `architecture.txt` |
| Mobile security tools | Tool home/about screens and authorized lab results | Tool-specific version or lab-result notes |

## Capturing command output

Run a command on your own device or computer, then copy its actual output into the matching file under `Outputs/`. Do not paste expected/example output as if it came from your device.

Examples of read-only verification commands:

```bash
# Root access check (run in an environment where su is available)
su -c id

# Android/Linux environment information
uname -a
uname -m

# Kali release information (inside NetHunter/Kali)
cat /etc/os-release

# Python and Git versions (where installed)
python --version
git --version
```

For Android device properties, use Android Settings > About phone, or collect appropriate non-sensitive details with ADB. Verify each result before recording it.

## Upload through GitHub website

1. Open your repository on GitHub.
2. Open the target folder, such as `Screenshots/root/` or `Outputs/root/`.
3. Select **Add file → Upload files**.
4. Select the real screenshot or `.txt` file from your computer and upload it.
5. Enter a descriptive commit message, such as `Add root verification evidence`.
6. Select **Commit changes**.
7. Repeat for the other evidence folders.

You can also upload multiple files to the same folder in one upload.

## Naming recommendations

Use clear names with lowercase letters and hyphens, for example:

- `about-phone.png`
- `lineageos-build.png`
- `magisk-status.png`
- `root-verification.png`
- `root-verification.txt`
- `nethunter-release.txt`

Use PNG or JPG for screenshots and TXT or MD for text evidence. Keep original files where possible and do not edit evidence in a way that changes what it proves. If you redact private details, state that the image has been redacted.

## Privacy and safety checklist

Before committing evidence, check that it does not reveal IMEI, serial number, phone number, email address, account identifiers, Wi-Fi passwords, API keys, access tokens, private keys, or personal notifications. Do not upload passwords, private keys, authentication tokens, or unredacted sensitive logs. Only include security-testing results from devices, apps, and systems you own or are authorized to assess.

## Evidence status

The folders and this guide are organizational templates only. They are not proof that a step was completed. Add your own genuine screenshots and command outputs. Do not claim a result until you have verified it on your device.
