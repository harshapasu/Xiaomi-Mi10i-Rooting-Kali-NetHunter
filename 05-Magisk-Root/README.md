# 05 — Magisk Root

## Recorded result

- Magisk application: version 31.1
- Root access: successfully established
- Bootloader: unlocked
- Zygisk: disabled in the last recorded configuration

## Verify root

From an authorized device shell:

```bash
su -c id
```

Expected identity includes:

```text
uid=0(root)
```

The exact output can include additional groups and context information.

## Important distinction

Installing the Magisk APK does not automatically mean the device is rooted. The project records root as working because root access was separately established.

## Security notes

- Review superuser prompts before granting access.
- Grant root only to trusted applications.
- Keep a record of installed modules and their sources.
- Re-check Zygisk and Magisk version after updates.
- Do not publish private app data or screenshots containing personal information.
