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
| `ClaspOs-0.3.2-windows.exe` | 87.13 MB | `8bf0dfdd39ab22ed551374c99667c28a4a682cdcb59c559f29326d1e5cf00ffe` |
| `ClaspOs-0.3.2-mac-applesilicon.dmg` | 99.95 MB | `e4a0da43803a77dcfafa10dc475aae0c9bbcb0b964a3a4101929e9971c052e0d` |
| `ClaspOs-0.3.2-mac-intel.dmg` | 104.22 MB | `5ccf8c353e974cde29b9febb79cece8b2874400d173f9e55e924791f2cfeadd5` |
| `ClaspOs-0.3.2-linux.AppImage` | 111.06 MB | `c7cec1eef863c79f1d703687f78acab9ce093754ae88bf04c8c38c96ff3b1c61` |
| `ClaspOs-0.3.2-mac-universal.dmg` | 177.04 MB | `ad2f92ceec52e5e3db534b4daec79bb435b263a828fe5978ad1f6e7e1fc5d690` |

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
