# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.7

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.7-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.7-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.7-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.7-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.7-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.7/ClaspOs-0.3.7-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.7)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.7-windows.exe` | 87.78 MB | `95867056c13ed8a700c93c1812811bcf6dac6cb9e8e8cc4b160065c1fbd7486c` |
| `ClaspOs-0.3.7-mac-applesilicon.dmg` | 100.77 MB | `5176dbab3b6aae6ae8e2047a5cb6d9cebdda65756f3c090aacf0d824b88ea7f5` |
| `ClaspOs-0.3.7-mac-intel.dmg` | 105.01 MB | `298dfc28656f696463531b3611f1761275ad34c7d4a503d1bb8ce398522ef0f8` |
| `ClaspOs-0.3.7-linux.AppImage` | 111.91 MB | `e225ee93cf9c3de7d7d21bf14101b669184845fc38f06cac4b27b34ae3b550da` |
| `ClaspOs-0.3.7-mac-universal.dmg` | 177.86 MB | `4951c5e4413ae2cd7587ded196d73c4cb2947eeea9f79dfab93544fc80b0c0d2` |

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
shasum -a 256 ClaspOs-0.3.7-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.7-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.7-windows.exe SHA256
```
