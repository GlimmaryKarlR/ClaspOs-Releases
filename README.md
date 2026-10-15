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
| `ClaspOs-0.2.8-windows.exe` | 86.96 MB | `0e4dd036e5a9a685c583ae2317325a1250bc8ca20fddfc03077272f1185b91d5` |
| `ClaspOs-0.2.8-mac-applesilicon.dmg` | 99.75 MB | `d4825e932c595560f64ee47e1c718b02348494cbc1fd3796ae76ef69215cd148` |
| `ClaspOs-0.2.8-mac-intel.dmg` | 104.00 MB | `d9fee978b0d9f576361463aeb9a9002fc1398d199c43549d8f3898f8acf3cfd0` |
| `ClaspOs-0.2.8-linux.AppImage` | 110.85 MB | `b3ad110cff8be21ad1543f638406cdd0859f88f4231b912dc8d328cb0cf5c4d6` |
| `ClaspOs-0.2.8-mac-universal.dmg` | 176.83 MB | `bb8292073211897da19db38aafe5ddc2da3454861ab62f923e8d6df79f4f7e9f` |

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
