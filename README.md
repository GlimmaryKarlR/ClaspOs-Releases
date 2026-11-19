# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.1

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.1-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.1/ClaspOs-0.6.1-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.1-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.1/ClaspOs-0.6.1-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.1-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.1/ClaspOs-0.6.1-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.1-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.1/ClaspOs-0.6.1-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.1-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.1/ClaspOs-0.6.1-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.1)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.1-windows.exe` | 89.69 MB | `762f193512d96ac7f0975aaea99b494192ca24c0a5d26bf51fb5ce2e6074f4cc` |
| `ClaspOs-0.6.1-mac-applesilicon.dmg` | 103.40 MB | `76eff7112e11d62de1560f510acf447ff4d0411947bdbd6b4c03f63c13165896` |
| `ClaspOs-0.6.1-mac-intel.dmg` | 107.66 MB | `e827f174f1bf9a67879601b78f69b940cfb0b2a946b8eccd2222e70885b6f330` |
| `ClaspOs-0.6.1-linux.AppImage` | 114.65 MB | `b5e955083a573c8a27120d72226b204d2a9cac8c13666060f7dce6c529385668` |
| `ClaspOs-0.6.1-mac-universal.dmg` | 180.50 MB | `6773a5a054aa858b1705e8304b365597a8581a00ff5486f45c364d9460ef84e1` |

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
shasum -a 256 ClaspOs-0.6.1-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.1-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.1-windows.exe SHA256
```
