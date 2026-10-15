# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.2.8

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.2.8-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.8/ClaspOs-0.2.8-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.2.8-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.8/ClaspOs-0.2.8-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.2.8-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.8/ClaspOs-0.2.8-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.2.8-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.8/ClaspOs-0.2.8-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.2.8-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.8/ClaspOs-0.2.8-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.2.8)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.2.8-windows.exe` | 86.95 MB | `bf7392a15fced208c3782fcd0c7c24687ee3f54d35f77830f170b10f697af386` |
| `ClaspOs-0.2.8-mac-applesilicon.dmg` | 99.74 MB | `927266e7c0773d3fbe0020ec1b4b181a99005e1acd8dff0e4a008652010edca0` |
| `ClaspOs-0.2.8-mac-intel.dmg` | 104.01 MB | `35d35089284c2622cf5cd0741e5fdd6c7a4d6a755f476b73271593ec5cb8ce15` |
| `ClaspOs-0.2.8-linux.AppImage` | 110.82 MB | `6ae639c0b87c63b2043d792e99abd6939a7bb6c863274d2a2069dec95a6f9f92` |
| `ClaspOs-0.2.8-mac-universal.dmg` | 176.82 MB | `4531fb606e84b65db52642246bd960ace25f3a84ee5fa94af8b3d0584c328561` |

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
shasum -a 256 ClaspOs-0.2.8-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.2.8-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.2.8-windows.exe SHA256
```
