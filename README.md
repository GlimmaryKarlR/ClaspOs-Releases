# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.5-windows.exe` | 87.69 MB | `97d1347f27e6ac3f97b3c036add2c4c0edae0d572c078ad4ecd997d90081c386` |
| `ClaspOs-0.3.5-mac-applesilicon.dmg` | 100.68 MB | `afed98b664202cdbc2e9f28650234fb051a24beba1771ec3f46831bbd6e92989` |
| `ClaspOs-0.3.5-mac-intel.dmg` | 104.89 MB | `1ed8c9e7997e7013e51f2269d5aa23b218f05ff06ecddb9516777959a0279991` |
| `ClaspOs-0.3.5-linux.AppImage` | 111.78 MB | `12cba2d04a6a9448d482abb5cffa4983989aabf7792121d054f67a62626a1438` |
| `ClaspOs-0.3.5-mac-universal.dmg` | 177.77 MB | `0df6065b0bdbafd6b7eaaeaf8be1653b6e8840abff73e671bf0625ffbd99dd57` |

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
shasum -a 256 ClaspOs-0.3.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.5-windows.exe SHA256
```
