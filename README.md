# Gonka Host Setup

A guided Windows app that takes a GPU server from bare metal to a registered, earning Gonka node.

## Install

Press the Windows key, type **PowerShell**, press Enter, then paste this and press Enter:

```powershell
irm https://raw.githubusercontent.com/gonkanetworkonboardinghub/gonka-host-setup/main/install.ps1 | iex
```

The app installs and opens by itself in about a minute. After that it keeps itself up to date.

### What the command does

[`install.ps1`](install.ps1) reads [`manifest.json`](manifest.json) to find the newest version and downloads that installer from this repository's [Releases](../../releases/latest). It checks the file's SHA-256 against the value published in the manifest and then runs it. The app installs for your Windows user only, so no admin rights are needed. Nothing else is downloaded or collected.

Prefer a regular download? Grab the installer from [Releases](../../releases/latest). Windows shows a "protected your PC" notice for downloaded installers it hasn't seen many times before; click **More info → Run anyway**.
