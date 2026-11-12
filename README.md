# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.5-windows.exe` | 88.06 MB | `aeee2a6f6e78cb6dc34f6af743fcff6b73671ca61296510343f4c510834a5d93` |
| `ClaspOs-0.5.5-mac-applesilicon.dmg` | 101.10 MB | `fd5b4d60120da8bf2b9a05a1c5f78862afd1c1f5f30cc19d26611d3e318eb783` |
| `ClaspOs-0.5.5-mac-intel.dmg` | 105.34 MB | `2846d556361fa5d1f76dbd343667fb2753c71d0812993bba45c38ccf32d5b165` |
| `ClaspOs-0.5.5-linux.AppImage` | 112.23 MB | `7e63d3c94b910c95d1c39c8eb3ac6ae3a94a7d2ccd587af3f9fcc5dbc1a41d9b` |
| `ClaspOs-0.5.5-mac-universal.dmg` | 178.17 MB | `3d9fac2b68d707be8ab1f267ab2cf4c083b04734518ede2499cc567d2ef1ca7a` |

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
shasum -a 256 ClaspOs-0.5.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.5-windows.exe SHA256
```
