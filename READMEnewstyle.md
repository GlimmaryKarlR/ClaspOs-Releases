# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.5/ClaspOs-0.4.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.5/ClaspOs-0.4.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.5/ClaspOs-0.4.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.5/ClaspOs-0.4.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.5/ClaspOs-0.4.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.5-windows.exe` | 87.86 MB | `0771a644c3ba9383d0848a66813377b4812380df46791f75e7332bb6f46e08c0` |
| `ClaspOs-0.4.5-mac-applesilicon.dmg` | 100.91 MB | `a2539c5dbfa790dbdabb259a0119df5e8535f61c4a22669944d95a830e6cd91e` |
| `ClaspOs-0.4.5-mac-intel.dmg` | 105.10 MB | `2dc469733d70eaf362b72f21e477a98cee19a7e786bda4a3b239cca3d5465f54` |
| `ClaspOs-0.4.5-linux.AppImage` | 112.00 MB | `ecbcb3cf5b052c255569d2b4e34bc7a89d61baf77d9fd5a50e06acca278e0684` |
| `ClaspOs-0.4.5-mac-universal.dmg` | 177.98 MB | `06348bec779dcb08cf4bfeebf4d1bacdb8082a3f7c775172bb90f3490d611d3d` |

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
shasum -a 256 ClaspOs-0.4.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.5-windows.exe SHA256
```
