# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.4

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.4-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.4/ClaspOs-0.3.4-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.4-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.4/ClaspOs-0.3.4-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.4-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.4/ClaspOs-0.3.4-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.4-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.4/ClaspOs-0.3.4-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.4-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.4/ClaspOs-0.3.4-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.4)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.4-windows.exe` | 87.21 MB | `ff93c43c8d0550cdad20d3ac9d22e2f9564f4ba80b08378d1ded9197e474285e` |
| `ClaspOs-0.3.4-mac-applesilicon.dmg` | 100.07 MB | `4762cb8411ce46966ca668c00f20fec740abeae038e02e6db73b64a59e0e9ea3` |
| `ClaspOs-0.3.4-mac-intel.dmg` | 104.30 MB | `918179b2ce39f7d34cb8b67a5665c2edfca9c70c43d2cbbe1b43883cebfd8474` |
| `ClaspOs-0.3.4-linux.AppImage` | 111.17 MB | `849c6cf62ab04379cf8048ef7a8dda7b8cbdc89a9f00265b8732447adba33920` |
| `ClaspOs-0.3.4-mac-universal.dmg` | 177.14 MB | `fc43bdadf85adce6bc12ca15e5600da0a8b2d6bc0abaf2a43ec940aa399faaab` |

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
shasum -a 256 ClaspOs-0.3.4-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.4-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.4-windows.exe SHA256
```
