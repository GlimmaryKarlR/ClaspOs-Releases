# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.2.6

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.2.6-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.6/ClaspOs-0.2.6-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.2.6-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.6/ClaspOs-0.2.6-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.2.6-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.6/ClaspOs-0.2.6-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.2.6-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.6/ClaspOs-0.2.6-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.2.6-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.6/ClaspOs-0.2.6-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.2.6)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.2.6-windows.exe` | 83.65 MB | `1f1a02b1119d9b54b5b5f3e3c27aa58bb3793da8456d82c3fa566492ea51381b` |
| `ClaspOs-0.2.6-mac-applesilicon.dmg` | 95.67 MB | `2bf139e1694ac3a60fbb6d42c7db8624dc7543bd5668ca6bce1edd7d29eafea6` |
| `ClaspOs-0.2.6-mac-intel.dmg` | 99.91 MB | `5e790ae76a4aac19b0b99f00c9ac0e78f60997e1de0c18b0b63b576c0a16489a` |
| `ClaspOs-0.2.6-linux.AppImage` | 106.75 MB | `9edadee186822ac8bc95852b3f14ced2647b65c9ada93da7d7e4a2c55c3090a7` |
| `ClaspOs-0.2.6-mac-universal.dmg` | 172.75 MB | `0d19eb29b547c2730f741cec58f386de948b4404b14d176b72a7dd5b9791b8e2` |

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
shasum -a 256 ClaspOs-0.2.6-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.2.6-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.2.6-windows.exe SHA256
```
