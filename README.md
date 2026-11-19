# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.2

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.2-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.2/ClaspOs-0.6.2-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.2-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.2/ClaspOs-0.6.2-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.2-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.2/ClaspOs-0.6.2-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.2-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.2/ClaspOs-0.6.2-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.2-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.2/ClaspOs-0.6.2-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.2)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.2-windows.exe` | 89.74 MB | `f5cbc5e523beb9efa2830f08a5227122e3e86da32c1ff497e5d7de21ac027033` |
| `ClaspOs-0.6.2-mac-applesilicon.dmg` | 103.54 MB | `05b04ea9f4f7ccc6941c2572d5a0aa1ed6b12f8a82c580922d657945daaecbe0` |
| `ClaspOs-0.6.2-mac-intel.dmg` | 107.72 MB | `e4a75f0df37c740cebbdc82044eb3803d9eff0cf8de94c0e23b05deffa4b5ee0` |
| `ClaspOs-0.6.2-linux.AppImage` | 114.74 MB | `56e6323dfc6c9bc0a1b84066aab7a65b745b43aba0c255502adc4c11420a906f` |
| `ClaspOs-0.6.2-mac-universal.dmg` | 180.59 MB | `a60bbab007a4bb4ca91f060f44c5d2e47c1efd22c16bc422ed9d281962b78e40` |

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
shasum -a 256 ClaspOs-0.6.2-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.2-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.2-windows.exe SHA256
```
