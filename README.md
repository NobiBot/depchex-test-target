# depchex-test-target

A test repository for [DepChex](https://github.com/NobiBot/DepChex) — a dependency confusion scanner for Python.

This repo contains dependency files with a mix of real packages and fictional private package names to verify DepChex's risk classification:

- **SAFE (green)**: packages like `flask`, `requests`, `django` — widely published on PyPI
- **CONFIRMED (red)**: fictional private packages like `acme-internal-auth` — not found on PyPI

## Usage

```bash
depchex --url https://github.com/NobiBot/depchex-test-target
```

Or scan locally:

```bash
git clone https://github.com/NobiBot/depchex-test-target.git
depchex --path /path/to/depchex-test-target
```
