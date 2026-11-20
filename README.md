# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.6.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.6.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.5/ClaspOs-0.6.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.6.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.5/ClaspOs-0.6.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.6.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.5/ClaspOs-0.6.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.6.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.5/ClaspOs-0.6.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.6.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.6.5/ClaspOs-0.6.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.6.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.6.5-windows.exe` | 89.87 MB | `484e80051c68d2edda3bc7c8c4b910e2d5157d2c43f48bed51262a57541507ef` |
| `ClaspOs-0.6.5-mac-applesilicon.dmg` | 103.69 MB | `aeb714429ed786245510356a42c112de7158d95c96ea5864de5aeb7bb2825632` |
| `ClaspOs-0.6.5-mac-intel.dmg` | 107.92 MB | `90060ae9303e4932bfc8dbf4284cbbfadb372bae9440f086d232318785db2791` |
| `ClaspOs-0.6.5-linux.AppImage` | 114.95 MB | `8aedaff5efd3d974447f5d8fb798a2cea4027c7dfc6c5afb66cdf74260739322` |
| `ClaspOs-0.6.5-mac-universal.dmg` | 180.81 MB | `eb7c304c8eac6fe1cce615dc8112f974208cabf65e98fd2bbecb5147488ee070` |

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
shasum -a 256 ClaspOs-0.6.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.6.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.6.5-windows.exe SHA256
```
