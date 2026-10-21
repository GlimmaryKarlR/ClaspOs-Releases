# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.1

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.1-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.1/ClaspOs-0.3.1-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.1-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.1/ClaspOs-0.3.1-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.1-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.1/ClaspOs-0.3.1-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.1-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.1/ClaspOs-0.3.1-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.1-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.1/ClaspOs-0.3.1-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.1)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.1-windows.exe` | 87.09 MB | `f19c23799db6a255bf286cc5476b3b1b2c08bda4e70e3e0fadab3fa34c90b998` |
| `ClaspOs-0.3.1-mac-applesilicon.dmg` | 99.94 MB | `f07136b157f89b563ce1b43481673c94ac97de1010260e75c602fdeceee99ab5` |
| `ClaspOs-0.3.1-mac-intel.dmg` | 104.16 MB | `e4719b065765bf3144cb5c175c197a1fa6a3e4db6cc513eddd756a134562f989` |
| `ClaspOs-0.3.1-linux.AppImage` | 111.02 MB | `f80e1c7d233774b610c7914db53c583e13a98969cdb296cda152f51b157b3f5c` |
| `ClaspOs-0.3.1-mac-universal.dmg` | 177.03 MB | `947c2a5b52bfef6e48b38029eb15c467d6109b1f02dc4d73cbd3a8b7ffdad693` |

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
shasum -a 256 ClaspOs-0.3.1-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.1-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.1-windows.exe SHA256
```
