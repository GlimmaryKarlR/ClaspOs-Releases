# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.7

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.7-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.7-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.7-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.7-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.7-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.7)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.7-windows.exe` | 87.78 MB | `540ee6be815aecfabf6a04a4ea0506c3570f061a72d8bd85af1a59fef799d820` |
| `ClaspOs-0.3.7-mac-applesilicon.dmg` | 100.77 MB | `2ef93bbd13adb721cc2ec3c8a1a2f8106a7dd1150d34432a7b1b5db7bff4ca23` |
| `ClaspOs-0.3.7-mac-intel.dmg` | 105.01 MB | `9b1129a913aeecb8ed6a452a623ccb4224def98c8bed28edd1d4d0667621db21` |
| `ClaspOs-0.3.7-linux.AppImage` | 111.91 MB | `f8c44abae1383ef21b16f9d27628728ab81508fd5baf6a51834ad9c80a331154` |
| `ClaspOs-0.3.7-mac-universal.dmg` | 177.86 MB | `634880f5556dad6605972abfff00460b53a2f83e4b4250c2eb7be3e109acced8` |

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
shasum -a 256 ClaspOs-0.3.7-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.7-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.7-windows.exe SHA256
```
