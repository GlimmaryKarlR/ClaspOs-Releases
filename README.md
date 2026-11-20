# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.7

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.7-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.7/ClaspOs-0.6.7-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.7-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.7/ClaspOs-0.6.7-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.7-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.7/ClaspOs-0.6.7-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.7-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.7/ClaspOs-0.6.7-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.7-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.7/ClaspOs-0.6.7-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.7)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.7-windows.exe` | 89.89 MB | `bc03794a68e28d91fbb54f0866c11962438bf548cf4e5274089b233e28ba2898` |
| `ClaspOs-0.6.7-mac-applesilicon.dmg` | 103.74 MB | `3f967adbdbc86f204e9054a25411ad636fa2bf60d489945a66795f354bf9f472` |
| `ClaspOs-0.6.7-mac-intel.dmg` | 107.98 MB | `6075bed4dd4041dd15034fe6f6d94b06e9d090be0411ac2301f79f9bdd170c48` |
| `ClaspOs-0.6.7-linux.AppImage` | 114.99 MB | `6e061610e85e43d1a86c0b57412558d5cab45566788a785ca82eb23ac35b0377` |
| `ClaspOs-0.6.7-mac-universal.dmg` | 180.83 MB | `6f92bf123be2bde0496d4246c9e340d9fb27559f0a666cd6d30b7b9d072ef313` |

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
shasum -a 256 ClaspOs-0.6.7-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.7-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.7-windows.exe SHA256
```
