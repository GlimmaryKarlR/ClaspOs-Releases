# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.8

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.8-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.8/ClaspOs-0.4.8-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.8-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.8/ClaspOs-0.4.8-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.8-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.8/ClaspOs-0.4.8-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.8-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.8/ClaspOs-0.4.8-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.8-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.8/ClaspOs-0.4.8-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.8)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.8-windows.exe` | 87.89 MB | `a10495af4b6109d0ba4452df353a8ece1d9a0e951b765830284daa7dc4c7e459` |
| `ClaspOs-0.4.8-mac-applesilicon.dmg` | 100.89 MB | `b75f817a1084a4d1ec1701cc56c49f6fe660054b69ca616aba8c4d968654cab6` |
| `ClaspOs-0.4.8-mac-intel.dmg` | 105.14 MB | `3f00b376a4c86f3f35a4edfd437db2169a75d857da9f877c51fd39faf70f1a9c` |
| `ClaspOs-0.4.8-linux.AppImage` | 112.03 MB | `e50a28347e6013f52bbd571a7af229a3390958f7859c01b3e1c924634e0da5a0` |
| `ClaspOs-0.4.8-mac-universal.dmg` | 178.00 MB | `e05717c3de21c228efcb6dd08b678636d76635c4bb34199c0f36678c0b10d037` |

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
shasum -a 256 ClaspOs-0.4.8-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.8-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.8-windows.exe SHA256
```
