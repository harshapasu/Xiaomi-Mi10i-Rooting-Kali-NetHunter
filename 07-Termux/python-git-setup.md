# Python and Git in Termux

```bash
pkg update
pkg install python git
python --version
git --version
```

For a Python project, use a virtual environment where supported:

```bash
python -m venv .venv
```

Activate it:

```bash
source .venv/bin/activate
```

Install only dependencies listed by the project and review package sources. Do not commit virtual environments, API keys or credentials.
