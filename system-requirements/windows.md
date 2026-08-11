# System requirements — Windows

*Current as of MyBI 26.1.0, 11 August 2026.*

## The short version

**Windows 10 version 1809 (build 17763) or later, 64-bit.** Windows 11 is fully supported.

## Architecture

| | Status |
|---|---|
| x64 (Intel, AMD) | Native |
| Arm64 (Windows on Arm) | Runs under the x64 emulation built into Windows 11 |
| 32-bit | Not supported |

A native Arm64 build is not published yet. On Windows 11 on Arm the x64 build runs through emulation,
which works but costs performance — and for an app whose job is querying data, that cost is more
noticeable than it would be in most software.

## Hardware

| | Minimum | Comfortable |
|---|---|---|
| Memory | 4 GB | 8 GB or more |
| Disk | 1 GB free | 5 GB or more with several projects open |

## What MyBI brings with it

- **The Visual C++ runtime** ships inside the app. Since 26.1.0 there is nothing to install first,
  and MyBI starts on a machine that has never run it before.
- **WebView2** is used for the interface. It is part of Windows 11 and present on essentially all
  supported Windows 10 machines through Microsoft's own updates.

## What is not available on Windows

Apple's on-device engines — Apple Intelligence, MLX, Apple's speech and vision frameworks — are
macOS only and are not shown on Windows. The assistant works with your own cloud API key, with a
local model runtime, or with a local AI CLI.

## Also worth knowing

- An internet connection is needed to sign in, to publish, to fetch language packs and colour
  palettes, and to check for updates. Building dashboards from your own files needs none.
- MyBI is distributed through the Microsoft Store.
