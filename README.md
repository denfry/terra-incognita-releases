# Terra: Incognita — Releases

Distribution repository for Terra Launcher and the Terra: Incognita modpack (closed source).

[![Discord](https://img.shields.io/badge/Discord-Join%20the%20community-5865F2?logo=discord&logoColor=white)](https://discord.gg/mVZcNUAGZt)

This repository holds the files Terra Launcher downloads: the launcher installer, the signed
release documents and the modpack's files. It contains no source code, and the launcher and pack
are not open source.

## Installation

1. Download the newest `TerraLauncher-<version>-setup.exe` from
   [Releases](https://github.com/denfry/terra-incognita-releases/releases?q=launcher&expanded=true).
2. Run it. The installer is not yet signed with a certificate, so Windows SmartScreen shows
   *"Windows protected your PC"*: click **More info**, then **Run anyway**. The `.sha256` file next
   to the installer lets you check the download.
3. Open Terra Launcher, type the player name you want, press **PLAY**. The launcher installs Java,
   Minecraft, NeoForge and the pack itself (about 1.5 GB the first time), then starts the game.

Microsoft sign-in is not available yet: the launcher plays under the name you type. Singleplayer
works; a server lets such a player in only with `online-mode=false`. Sign-in arrives with a later
launcher version, and installed launchers update themselves.

## Requirements

- Windows 10/11, 64-bit
- 8 GB RAM (the game gets 6 GB)
- About 4 GB of disk space

## Repository contents

| Where | What |
|---|---|
| Releases `launcher-v<version>` | the installer and its checksum |
| Releases `objects-00` … `objects-ff` | the pack's files, one asset per file, named by SHA-256 |
| branch `gh-pages` | the trust root, channel pointers and signed manifests the launcher reads |

Every file the launcher installs is named, with its hash, in a manifest signed by the project's
keys; the launcher trusts nothing else. Third-party mods keep their own licences; the launcher
downloads the ones whose licence does not allow redistribution straight from their authors.

## Community

Questions and feedback: [Discord](https://discord.gg/mVZcNUAGZt).
