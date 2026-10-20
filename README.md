# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.0

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.0-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.0-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.0-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.0-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.0-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.0/ClaspOs-0.3.0-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.0)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.0-windows.exe` | 87.07 MB | `6b0b675602ef54c1d603255210129bb27bec31a08965bd4d5949e0c38d8cecbb` |
| `ClaspOs-0.3.0-mac-applesilicon.dmg` | 99.93 MB | `1e707f70762ecbe9c35ed9198b5a7df8354c09c97b3f620589056a3b6d1d5490` |
| `ClaspOs-0.3.0-mac-intel.dmg` | 104.12 MB | `0d7fe0cd80243798f23a5aa1439478a7e7a0b1c846834c46e9b0570d32698ca9` |
| `ClaspOs-0.3.0-linux.AppImage` | 110.99 MB | `c8a3c42e2a4fbad04274d50c2f4c35cfeb24f159bed9485b3bf8d96f4aa73930` |
| `ClaspOs-0.3.0-mac-universal.dmg` | 176.97 MB | `ecf8546bb9b23573ff30cc8f7cf8430e1cf7e99aeba4c01870d5f5e7d0cd486e` |

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
shasum -a 256 ClaspOs-0.3.0-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.0-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.0-windows.exe SHA256
```
