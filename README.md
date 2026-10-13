# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.2.7

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.2.7-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.7/ClaspOs-0.2.7-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.2.7-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.7/ClaspOs-0.2.7-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.2.7-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.7/ClaspOs-0.2.7-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.2.7-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.7/ClaspOs-0.2.7-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.2.7-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.7/ClaspOs-0.2.7-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.2.7)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.2.7-windows.exe` | 86.93 MB | `700a8871dc920e3ecc6abb9c2b6614c2e4f21a8962ec33ace067869e9cab9e72` |
| `ClaspOs-0.2.7-mac-applesilicon.dmg` | 99.70 MB | `4eb0db7b284e834e8a4fbf34a6abdc541bd2753c0a0fc35d072f1e435366052c` |
| `ClaspOs-0.2.7-mac-intel.dmg` | 103.96 MB | `a6ddcd16b67cc13e1b3078c3394bad11399beacc8eea24ce3db72010eca7a6fc` |
| `ClaspOs-0.2.7-linux.AppImage` | 110.80 MB | `9998212f24a608d685ea64738530a0e365da2de6c1d1e93226b18b8cb7abbf66` |
| `ClaspOs-0.2.7-mac-universal.dmg` | 176.81 MB | `24ea637c7513222504bd03743d4f4eedaced9e3d2e09ca983aa89c0ba52553fc` |

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
shasum -a 256 ClaspOs-0.2.7-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.2.7-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.2.7-windows.exe SHA256
```
