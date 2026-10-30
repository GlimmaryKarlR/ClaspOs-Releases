# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.8

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.8-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.8/ClaspOs-0.3.8-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.8-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.8/ClaspOs-0.3.8-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.8-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.8/ClaspOs-0.3.8-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.8-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.8/ClaspOs-0.3.8-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.8-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.8/ClaspOs-0.3.8-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.8)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.8-windows.exe` | 87.78 MB | `fb1ce524cc7aac4d6bc1e5520d6ef73c769e42f37ecdc723808ac6f8b1331e5b` |
| `ClaspOs-0.3.8-mac-applesilicon.dmg` | 100.77 MB | `fa217c33fca4bdb2e35bb2ab444af70296b22238748c4c77e019ad55361fe232` |
| `ClaspOs-0.3.8-mac-intel.dmg` | 105.01 MB | `2f30b365ca135f0a15053e82948eb080ec269e355d12435896e7307c3e4b969a` |
| `ClaspOs-0.3.8-linux.AppImage` | 111.91 MB | `dbbbf8e128e05e4d3f86ca1b2a490f18a73834a510535bc686b84252addeba3b` |
| `ClaspOs-0.3.8-mac-universal.dmg` | 177.89 MB | `83b08600129e0c3f22fa0344affe27e90ced4e1e6ad8ca63c25d188d75b8de35` |

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
shasum -a 256 ClaspOs-0.3.8-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.8-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.8-windows.exe SHA256
```
