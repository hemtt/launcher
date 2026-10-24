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
hemtt versions list
```

Install the latest HEMTT release:

```bash
hemtt versions install latest
```

Update to the latest HEMTT release (the newest installed version is used by default):

```bash
hemtt update
```

Remove a specific HEMTT version:

```bash
hemtt versions remove <version>
```

Run a specific HEMTT version:

```bash
hemtt +<version> build
```

Test a HEMTT PR:

```bash
hemtt +pr/<pr-number> build
```

Every HEMTT process started by the launcher has `HEMTT_FROM_LAUNCHER=1` set in its environment.

The launcher checks for a newer HEMTT Launcher release every 12 hours and prints a notice when one is available. It never replaces itself, so download new launcher versions from the [releases page](https://github.com/hemtt/launcher/releases).
