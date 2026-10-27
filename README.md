# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.6

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.6-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.6/ClaspOs-0.3.6-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.6-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.6/ClaspOs-0.3.6-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.6-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.6/ClaspOs-0.3.6-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.6-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.6/ClaspOs-0.3.6-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.6-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.6/ClaspOs-0.3.6-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.6)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.6-windows.exe` | 87.75 MB | `614cb36573681a5fdba4acf186ec39a8d3e53110ff88e5d1874ffd9681a598f4` |
| `ClaspOs-0.3.6-mac-applesilicon.dmg` | 100.72 MB | `234a1f77f7254885a0b9fc5ca676d540d878592e3c8c816d67bc7e6d185f7fe2` |
| `ClaspOs-0.3.6-mac-intel.dmg` | 104.97 MB | `c66f19e0b23ae658685cdf19dca7a67cea9488e5079803c91194a5cc7d6b07d0` |
| `ClaspOs-0.3.6-linux.AppImage` | 111.86 MB | `33c7b018e27a17f949795e12bcb7322b68ca833d16f9cc3ff816f8b9abaaf8c7` |
| `ClaspOs-0.3.6-mac-universal.dmg` | 177.80 MB | `5a49fdadd44c7d40f36549585b8df52cf782832e6f9952b4f2e1da1ab0e5dc89` |

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
shasum -a 256 ClaspOs-0.3.6-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.6-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.6-windows.exe SHA256
```
