# HEMTT Launcher

HEMTT Launcher is a tool to manage and launch HEMTT instances efficiently.

## Installation

### Windows

```powershell
winget install hemtt
```

### Linux & MacOS

```bash
curl -sSf https://hemtt.dev/install.sh | sh
```

## Usage

List all installed HEMTT versions:

```bash
hemtt version list
```

Remove a specific HEMTT version:

```bash
hemtt version remove <version>
```

Run a specific HEMTT version:

```bash
hemtt +<version> build
```

Test a HEMTT PR:

```bash
hemtt +pr/<pr-number> build
```
