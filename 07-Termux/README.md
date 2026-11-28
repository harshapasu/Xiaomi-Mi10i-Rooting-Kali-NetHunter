# 07 — Termux

Termux provides a terminal environment on Android. It is not identical to a conventional desktop Linux installation.

## Package setup

```bash
pkg update
pkg upgrade
pkg install git python wget curl nano
```

## Storage permission

If shared storage access is required:

```bash
termux-setup-storage
```

Approve the Android permission prompt.

## Environment checks

```bash
whoami
pwd
uname -a
python --version
git --version
```

## Notes

- Use Termux packages from its supported repositories.
- Keep Termux and its plugins from compatible distribution sources.
- Some desktop Linux services and kernel features are unavailable in Android's app environment.
- Keep project files in a location that is accessible to both Termux and your intended Git workflow.
