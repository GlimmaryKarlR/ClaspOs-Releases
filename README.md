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
| `ClaspOs-0.4.8-windows.exe` | 87.88 MB | `b8263169cde94c3228305d598d76acb8dc59bd1b00a54b2b9a4ba893e4b397eb` |
| `ClaspOs-0.4.8-mac-applesilicon.dmg` | 100.89 MB | `3e0e546b4926229a1d19bf45915b5a13c7b4493b8fa67e4b4bb632eef81f551f` |
| `ClaspOs-0.4.8-mac-intel.dmg` | 105.14 MB | `13535b8e7ca97394f4a6c50768c674092cf67ee53488cde7d41e035cfa9df664` |
| `ClaspOs-0.4.8-linux.AppImage` | 112.03 MB | `8c63dad164337a8534df618d5deb9ed18a0bd0641d9f4c979a755058640123be` |
| `ClaspOs-0.4.8-mac-universal.dmg` | 178.00 MB | `312d984e75e471367e6d7df8be9b5a12ea9f28e1307e10a4bf003411022c5b63` |

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
