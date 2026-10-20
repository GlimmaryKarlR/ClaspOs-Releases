# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.0

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.0-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.0-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.0-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.0-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.0-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.0)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.0-windows.exe` | 87.05 MB | `fa20ee7846749b20695c73a9f5fb365192efd024fec56cc4f230225c505d4882` |
| `ClaspOs-0.3.0-mac-applesilicon.dmg` | 99.87 MB | `c77c33c48abe2f3adc9015e5f71cce7c1a26d1b4a521b86d88532f1381e67042` |
| `ClaspOs-0.3.0-mac-intel.dmg` | 104.12 MB | `897d31531a5b6f3c94c9a46f58c89768bf563264606ea1c39c321524096a0727` |
| `ClaspOs-0.3.0-linux.AppImage` | 110.97 MB | `02130c2c9e8c810d7e27c10edfc32cd3e7d4bfa17d750ca259790cf8f4d09b07` |
| `ClaspOs-0.3.0-mac-universal.dmg` | 176.93 MB | `ee40a1a2c41bb99992ce47d245a92234ac5467dbcccea2ac5538e2eda7c3d8f8` |

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
shasum -a 256 ClaspOs-0.3.0-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.0-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.0-windows.exe SHA256
```
