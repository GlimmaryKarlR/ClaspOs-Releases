# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.3

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.3-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.3/ClaspOs-0.3.3-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.3-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.3/ClaspOs-0.3.3-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.3-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.3/ClaspOs-0.3.3-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.3-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.3/ClaspOs-0.3.3-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.3-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.3/ClaspOs-0.3.3-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.3)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.3-windows.exe` | 87.18 MB | `a7f96db9a2b5dfade35b80fc3a98094a14dfbe5dcd1610df87c757b90727e786` |
| `ClaspOs-0.3.3-mac-applesilicon.dmg` | 100.00 MB | `9c75cb6f6d7a1adb1e4bd08f945ed4a4113774f60bb9d3ab4ef854a193e79109` |
| `ClaspOs-0.3.3-mac-intel.dmg` | 104.25 MB | `193414622dcb908a47452873d7ad9a4721266004c0dde9dd24f3e247ae68da6b` |
| `ClaspOs-0.3.3-linux.AppImage` | 111.13 MB | `76fdb1a1f31c28e7c1058aee872288ce92aeb5c6c1ed738d8eb8c3dd18b01997` |
| `ClaspOs-0.3.3-mac-universal.dmg` | 177.09 MB | `66f10a22f7e70c11831fb276e5281a7e0a0b0aec78bdde3ede683cc5cf9133a3` |

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
shasum -a 256 ClaspOs-0.3.3-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.3-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.3-windows.exe SHA256
```
