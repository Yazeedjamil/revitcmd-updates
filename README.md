# revitcmd-updates

The update feed for the **Revit Command Bar**, a Revit add-in by Yazeed Hammad.

**There is no source code here.** This repository holds three things and nothing else:

- `latest.json` — what the installed add-in reads to find out whether a newer version
  exists. Every entry carries a SHA-256, and the add-in refuses any download whose
  hash does not match.
- **Releases** — the installer (`RevitCmd-Setup-<version>.exe`) and the logic packages
  (`logic-2023-<version>.zip` for Revit 2023–2024, `logic-2025-<version>.zip` for
  Revit 2025–2026) for each version.
- This README.

## Installing

Download the newest `RevitCmd-Setup-<version>.exe` from
[Releases](https://github.com/Yazeedjamil/revitcmd-updates/releases) and run it. It
installs for the current user only — no administrator rights are needed — and
registers itself with every Revit 2023–2026 it finds on the machine.

The installer is not code-signed yet, so Windows SmartScreen will warn the first few
times. "More info" → "Run anyway".

## Updating

The add-in checks this feed itself and installs updates quietly when Revit closes.
There is normally nothing to do.

## Access

The Command Bar needs a sign-in, and sign-in is by invitation while it is in beta.
Ask Yazeed for access.
