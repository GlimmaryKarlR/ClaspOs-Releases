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
| `ClaspOs-0.3.7-windows.exe` | 87.78 MB | `2d540b9aadb3944568df6e5e43262e0f63f1f32d6110cdfb6e73a61ba0de8ddb` |
| `ClaspOs-0.3.7-mac-applesilicon.dmg` | 100.77 MB | `cbb52eb0c4761d48bbb9eee50180a774d20eaf6f185e18ac869edb3a2eb51edd` |
| `ClaspOs-0.3.7-mac-intel.dmg` | 105.01 MB | `ca8bae805d8cc83ec82960e3e12db4106d43d28d1a2f65c84e807b875963e2c7` |
| `ClaspOs-0.3.7-linux.AppImage` | 111.90 MB | `76ad30e4c373473fbcb6156fa2bbb977a2360de3a2a9050e1d20fca3d0d059c1` |
| `ClaspOs-0.3.7-mac-universal.dmg` | 177.88 MB | `b70e08c6d718786bdfc9327e78bfe04980fef68b52e8a021f74b7ed18d08e857` |

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
