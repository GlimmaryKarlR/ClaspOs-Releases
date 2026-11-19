# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.3

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.3-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.3/ClaspOs-0.6.3-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.3-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.3/ClaspOs-0.6.3-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.3-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.3/ClaspOs-0.6.3-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.3-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.3/ClaspOs-0.6.3-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.3-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.3/ClaspOs-0.6.3-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.3)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.3-windows.exe` | 89.79 MB | `c40e1f93cd40e26dd04d57fb40f03488da7a404fefe0dcc55678a2c80ebd113b` |
| `ClaspOs-0.6.3-mac-applesilicon.dmg` | 103.60 MB | `44f96d993552034106f933db69b5ca72004818a18e73ecdca1f7e392b15803ab` |
| `ClaspOs-0.6.3-mac-intel.dmg` | 107.84 MB | `0eb694aca7b0e28f8c626278e5c18041954286e34ef23e470d7bef9dce3f2809` |
| `ClaspOs-0.6.3-linux.AppImage` | 114.84 MB | `15d5a9a722557a8ea6cf2dda360a88841bf1c1529c01529c8b7209878984f886` |
| `ClaspOs-0.6.3-mac-universal.dmg` | 180.66 MB | `b0e7a7a1d0096105b629096ba1009405c7e3e0e40f6ccec898f7d47cc0a1b5c0` |

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
shasum -a 256 ClaspOs-0.6.3-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.3-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.3-windows.exe SHA256
```
