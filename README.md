# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.1

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.1-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.1/ClaspOs-0.4.1-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.1-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.1/ClaspOs-0.4.1-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.1-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.1/ClaspOs-0.4.1-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.1-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.1/ClaspOs-0.4.1-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.1-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.1/ClaspOs-0.4.1-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.1)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.1-windows.exe` | 87.82 MB | `aa8c96489f858f317af360d3fe9f4e06ee977e71ed34e134e484bb11f2ed1329` |
| `ClaspOs-0.4.1-mac-applesilicon.dmg` | 100.81 MB | `e6c11596b1541703c07ae5108ea7f16b7993149761e82175d335825385ae3381` |
| `ClaspOs-0.4.1-mac-intel.dmg` | 105.08 MB | `fc3c44e5381425d2c3d6674fbefc10ffa036be0a99d7217584cbe9e7409c69f3` |
| `ClaspOs-0.4.1-linux.AppImage` | 111.95 MB | `ff8a4b96576c4347a9fd6829b08810b1026ca367b8d3668a5087b1e9415adb1d` |
| `ClaspOs-0.4.1-mac-universal.dmg` | 177.88 MB | `9dfac50afa8163b3432a0151a093d8a036608d7534b59a13e34f0feb60ab2393` |

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
shasum -a 256 ClaspOs-0.4.1-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.1-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.1-windows.exe SHA256
```
