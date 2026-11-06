# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.7

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.7-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.7/ClaspOs-0.4.7-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.7-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.7/ClaspOs-0.4.7-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.7-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.7/ClaspOs-0.4.7-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.7-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.7/ClaspOs-0.4.7-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.7-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.7/ClaspOs-0.4.7-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.7)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.7-windows.exe` | 87.88 MB | `910602a628ecf9b9b9702dcbe3a408ceb0af5825c7a090143237df0a6a454e5f` |
| `ClaspOs-0.4.7-mac-applesilicon.dmg` | 100.89 MB | `86487cfd1f64d81ee32af6319fe4a4f297afcadac30444a45980c7b663a3a599` |
| `ClaspOs-0.4.7-mac-intel.dmg` | 105.14 MB | `b04dbc84e2003add43ec31a4ca829d15a1a3cd0bbee086256cd7ccecb29addaf` |
| `ClaspOs-0.4.7-linux.AppImage` | 112.03 MB | `48784890072078a6d79011c96879bdd1f7ae0d7624bbd2495dde879f0383e211` |
| `ClaspOs-0.4.7-mac-universal.dmg` | 177.99 MB | `ee9662cae2b2d2430221f0b17be27c6eaec3fc3ee5f376fc8d563b7d2dcedae6` |

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
shasum -a 256 ClaspOs-0.4.7-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.7-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.7-windows.exe SHA256
```
