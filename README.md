# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.9

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.9-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.9/ClaspOs-0.6.9-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.9-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.9/ClaspOs-0.6.9-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.9-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.9/ClaspOs-0.6.9-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.9-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.9/ClaspOs-0.6.9-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.9-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.9/ClaspOs-0.6.9-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.9)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.9-windows.exe` | 89.89 MB | `ea557ef7639ed7840b4cb149ca4a837695304b3243fb51dfb7a0288d1fc21b7a` |
| `ClaspOs-0.6.9-mac-applesilicon.dmg` | 104.05 MB | `03df209162316a5b4f6962dc46c6af93b227f04a6dbe88163e730e2c5ef32751` |
| `ClaspOs-0.6.9-mac-intel.dmg` | 108.32 MB | `ce5af4e710e9b28d3453216de50fe9afee9245ad1023fd6ea36f37ef044084d1` |
| `ClaspOs-0.6.9-linux.AppImage` | 115.35 MB | `2be5665d50c9dbbc4f19a1046a0b57a9b2380885e947477c1e517eb2ddde4974` |
| `ClaspOs-0.6.9-mac-universal.dmg` | 181.14 MB | `3d68151cfe19c9d8cd5bcc0c9a9bbb7234bd2d961becebb6512f62d0d8f70cf8` |

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
shasum -a 256 ClaspOs-0.6.9-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.9-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.9-windows.exe SHA256
```
