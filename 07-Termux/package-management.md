# Termux Package Management

Update package metadata and installed packages:

```bash
pkg update
pkg upgrade
```

Install common utilities:

```bash
pkg install git python wget curl nano
```

Inspect installed packages:

```bash
pkg list-installed
```

If a package installation fails, record the exact error, repository configuration, Termux version and date. Do not mix instructions for obsolete Termux builds with current installations.
