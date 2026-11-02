# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.2

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.2-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.2/ClaspOs-0.4.2-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.2-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.2/ClaspOs-0.4.2-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.2-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.2/ClaspOs-0.4.2-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.2-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.2/ClaspOs-0.4.2-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.2-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.2/ClaspOs-0.4.2-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.2)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.2-windows.exe` | 87.85 MB | `d8029ae2569873fcad8e436cba111cddd8693f75d7e9daffb6fe238c2d5b8ae4` |
| `ClaspOs-0.4.2-mac-applesilicon.dmg` | 100.86 MB | `976eed400555a18cab56565946c54f1d52d2de40696810ef0eb8aabe8361b176` |
| `ClaspOs-0.4.2-mac-intel.dmg` | 105.08 MB | `e6e477474ebda5ad535ce22821f174ad5f05eaafc2d40a59756c4394ea99ceaf` |
| `ClaspOs-0.4.2-linux.AppImage` | 111.98 MB | `71eaa651a6f59470c9ef75e1e62255eebcfab7aab9ee3ab69fd9b991b8b433a4` |
| `ClaspOs-0.4.2-mac-universal.dmg` | 177.94 MB | `65b9b3a4dda8324352628bba5bc6a7ad74720a18e885f75ce698494c37b4d8ff` |

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
shasum -a 256 ClaspOs-0.4.2-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.2-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.2-windows.exe SHA256
```
