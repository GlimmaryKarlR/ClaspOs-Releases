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
| `ClaspOs-0.4.7-windows.exe` | 87.88 MB | `aae131b7a9b787bd1aaf165137b238eba4688908d2d636eeb4c365faa665d200` |
| `ClaspOs-0.4.7-mac-applesilicon.dmg` | 100.92 MB | `aaa3c4585f2eb506615fefce0fd37018726a1b766d24eb11b3884accf3be5d45` |
| `ClaspOs-0.4.7-mac-intel.dmg` | 105.14 MB | `8b213358eab47894000a76414a855fcc28c526e97a054167664b6884049bacf0` |
| `ClaspOs-0.4.7-linux.AppImage` | 112.03 MB | `206bc6fc065b3297974fd8df2cdf8e3bd53b31bd5a337f17a570a853b91b2a65` |
| `ClaspOs-0.4.7-mac-universal.dmg` | 177.98 MB | `6746d4d7179ce1c188c9c1dce5c54f48372e3bd0817332d15f3d18d5e31e4ba5` |

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
