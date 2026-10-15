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
| `ClaspOs-0.2.8-windows.exe` | 86.94 MB | `6010f4a89afb0cf81bb70b3bc995e0a89402e0c18b4a66799b12ae41e983914d` |
| `ClaspOs-0.2.8-mac-applesilicon.dmg` | 99.72 MB | `2007dc374648a9859cdb1be6b4b19cb4b2cf055d0683815f3d9153d1e00501c1` |
| `ClaspOs-0.2.8-mac-intel.dmg` | 104.02 MB | `4821c9b3f3ca56341a53a0ffddbbc6e43df0dcafc906cdcedb5c586ee2f93a06` |
| `ClaspOs-0.2.8-linux.AppImage` | 110.83 MB | `5fe6393434852f04b5092387f8c301ff0b7dd8112b6fddd13447357c0e954b3a` |
| `ClaspOs-0.2.8-mac-universal.dmg` | 176.79 MB | `1b31e1a40a4a615af0fbb5bc225555905e8a0d2506bc4acf5696aa70e17caff4` |

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
