# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.2

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.2-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.2/ClaspOs-0.5.2-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.2-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.2/ClaspOs-0.5.2-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.2-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.2/ClaspOs-0.5.2-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.2-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.2/ClaspOs-0.5.2-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.2-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.2/ClaspOs-0.5.2-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.2)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.2-windows.exe` | 87.96 MB | `67f8587424fdcebeef2ca65c8248c992ca94a0ecf62cd70dda7aa8f4aec335bc` |
| `ClaspOs-0.5.2-mac-applesilicon.dmg` | 100.99 MB | `0a2e0e8ab739f238071bbf86b06bcc46524c7076e78e570567305ea3e1da062e` |
| `ClaspOs-0.5.2-mac-intel.dmg` | 105.22 MB | `3f9cf9fd07a6f00615deabfe41c47b805d25d84a8e82e5c94d68c4236034e6d2` |
| `ClaspOs-0.5.2-linux.AppImage` | 112.13 MB | `ee2bf2773ebd779e0650af9e5b8744d61bd2800c906c616d03c6bd255f514761` |
| `ClaspOs-0.5.2-mac-universal.dmg` | 178.09 MB | `815542c19d9276d50038dc1c6f4853a3527e95f361a5db65ac7e5cfc5ec949f5` |

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
shasum -a 256 ClaspOs-0.5.2-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.2-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.2-windows.exe SHA256
```
