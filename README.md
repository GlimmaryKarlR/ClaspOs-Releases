# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.0

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.0-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.0/ClaspOs-0.6.0-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.0-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.0/ClaspOs-0.6.0-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.0-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.0/ClaspOs-0.6.0-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.0-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.0/ClaspOs-0.6.0-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.0-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.0/ClaspOs-0.6.0-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.0)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.0-windows.exe` | 89.67 MB | `c3557b6d18941ff1c2ccb6efcaa090be19c3e58494b6a6d3560efe2f92ce0969` |
| `ClaspOs-0.6.0-mac-applesilicon.dmg` | 103.38 MB | `05ef1bfe77b37f3ac53bfe931d908b8cd85006db61aa75bc40bad719a33cc73f` |
| `ClaspOs-0.6.0-mac-intel.dmg` | 107.61 MB | `024932995886ccae582d1cd205ebc4766c09a6f182a30bc439c5fca4d3d1f883` |
| `ClaspOs-0.6.0-linux.AppImage` | 114.62 MB | `552e552c4601cde1311146601c738405ce22e325dda94059027a2a8c671609d6` |
| `ClaspOs-0.6.0-mac-universal.dmg` | 180.48 MB | `63d1cb6666e2b802e4924f3067d2acef90d691b100498034a08ad0c84e522087` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`
* **Windows (Command Prompt)**: `certutil -hashfile <filename> SHA256`


---

## Integrity Verification Guide

To verify your downloaded binary matches the official build byte-for-byte before running:

### macOS / Linux
```bash
# Test specific binary:
shasum -a 256 ClaspOs-0.6.0-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.0-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.0-windows.exe SHA256
```
