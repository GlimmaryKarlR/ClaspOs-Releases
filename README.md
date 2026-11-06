# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.6

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.6-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.6/ClaspOs-0.4.6-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.6-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.6/ClaspOs-0.4.6-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.6-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.6/ClaspOs-0.4.6-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.6-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.6/ClaspOs-0.4.6-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.6-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.6/ClaspOs-0.4.6-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.6)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.6-windows.exe` | 87.86 MB | `18848133d7e1798d8f75ce96c059725adfaaf9d27d9d3c4af30f904d2e6f175d` |
| `ClaspOs-0.4.6-mac-applesilicon.dmg` | 100.92 MB | `76e6614578cf3273fd6d7eb0e89193c639c24ea75018adc6bc7b956e1554a5a5` |
| `ClaspOs-0.4.6-mac-intel.dmg` | 105.11 MB | `c651df36508ae546273cf99a142785ba2d00db7af3c79404f71df63474629523` |
| `ClaspOs-0.4.6-linux.AppImage` | 112.00 MB | `f8910bb55151fcaae8659613901e3e48420714f0c69d4eef2b1ffdcbdf7b838d` |
| `ClaspOs-0.4.6-mac-universal.dmg` | 177.98 MB | `564206c3c1b07cba41b935d63ddde3146768afc1e971a499e0399467f6ed004a` |

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
shasum -a 256 ClaspOs-0.4.6-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.6-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.6-windows.exe SHA256
```
