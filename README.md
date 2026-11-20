# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.6

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.6-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.6/ClaspOs-0.6.6-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.6-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.6/ClaspOs-0.6.6-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.6-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.6/ClaspOs-0.6.6-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.6-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.6/ClaspOs-0.6.6-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.6-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.6/ClaspOs-0.6.6-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.6)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.6-windows.exe` | 89.87 MB | `2c76dc39e9c03515cfe1fb025a9de8a8f556440ffb1fcf515c1a0a9709b52fb3` |
| `ClaspOs-0.6.6-mac-applesilicon.dmg` | 103.68 MB | `2899c04bbf71972d67805ae643844cdde3ba50e0614c282366ea9507b94432a2` |
| `ClaspOs-0.6.6-mac-intel.dmg` | 107.92 MB | `8796934e8a9495c86384ea3b2821cb21ad84c1e8d000a5bed0342bb2c9a9d6a5` |
| `ClaspOs-0.6.6-linux.AppImage` | 114.94 MB | `e9e47ed4edc5fe41b1dd26e2aba0ee9a73e5291baf1fa07d91034045aaa12734` |
| `ClaspOs-0.6.6-mac-universal.dmg` | 180.81 MB | `e3611e407d5ca05caf922a26faadc90d992bc8a17de3c86fc665fc93faa168c7` |

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
shasum -a 256 ClaspOs-0.6.6-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.6-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.6-windows.exe SHA256
```
