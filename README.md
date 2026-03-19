# Cleave — Releases

Release binaries for [Cleave](https://github.com/TimoHanisch/cleave), a local WoW combat log analyzer.

## Download

Download the latest release for your platform:

| Platform | Download |
|----------|----------|
| macOS (Apple Silicon) | [.tar.gz](https://github.com/TimoHanisch/cleave-releases/releases/latest) |
| Windows x64 | [.msi](https://github.com/TimoHanisch/cleave-releases/releases/latest) (installer) or
[.zip](https://github.com/TimoHanisch/cleave-releases/releases/latest) (portable) |

Or browse all versions on the [Releases](https://github.com/TimoHanisch/cleave-releases/releases) page.

## Quick start

1. Download and run `cleave` (macOS) or install the `.msi` (Windows)
2. Cleave opens your browser to `http://localhost:8080`
3. Drag and drop a `WoWCombatLog.txt` onto the import area, or enable the file watcher for auto-detection

## Auto-update

Cleave checks this repo for new versions automatically. When an update is available, you'll see a notification in the app. Downloads 
are verified with SHA256 checksums before install.

## What is Cleave?

A local, privacy-first WoW combat log analyzer for Midnight (12.x). Parses combat logs, stores events in SQLite, and serves an
interactive web UI — all from a single binary. Your data never leaves your machine.

Features include damage/healing/damage taken breakdowns, buff uptime tracking, cast timelines, death recaps, rotation analysis, player
comparison, progress reports, live combat overlay, and more.

## Checksums

Every release includes `.sha256` files for verification:

```bash
# macOS
shasum -a 256 -c cleave-*.tar.gz.sha256

# Windows (PowerShell)
Get-FileHash cleave-*.msi | Format-List
```
