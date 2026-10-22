# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.2

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.2-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.2/ClaspOs-0.3.2-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.2-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.2/ClaspOs-0.3.2-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.2-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.2/ClaspOs-0.3.2-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.2-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.2/ClaspOs-0.3.2-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.2-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.2/ClaspOs-0.3.2-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.2)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.2-windows.exe` | 87.13 MB | `79fe4ece73cfb77ff4ab4dc02a41f75db456b98b26bf2a586bf8695b17fe77bb` |
| `ClaspOs-0.3.2-mac-applesilicon.dmg` | 99.95 MB | `ba2b5df81e7d1bbbd2171571350f747714125ce3f864ba6816de11ff6a467b83` |
| `ClaspOs-0.3.2-mac-intel.dmg` | 104.24 MB | `7492eb9e6092c9f594cd5b58024e717877dc05ed12b846f360a45664cf32205a` |
| `ClaspOs-0.3.2-linux.AppImage` | 111.07 MB | `072c8776826bb83492484df6ca957801ff69b1f614f9f67f5e0b3559a340bb89` |
| `ClaspOs-0.3.2-mac-universal.dmg` | 177.03 MB | `3392938c6c3216a063ddb25bcdce59dd0dc5392028d76dbbdf9f713046c8146a` |

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
shasum -a 256 ClaspOs-0.3.2-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.2-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.2-windows.exe SHA256
```
