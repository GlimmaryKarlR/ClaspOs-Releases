# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.9

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.9-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.9/ClaspOs-0.3.9-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.9-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.9/ClaspOs-0.3.9-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.9-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.9/ClaspOs-0.3.9-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.9-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.9/ClaspOs-0.3.9-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.9-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.9/ClaspOs-0.3.9-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.9)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.9-windows.exe` | 87.81 MB | `73b3fef73ec3329b379bfbff31e00295b2973aca0aa29a34266904af8d1238b8` |
| `ClaspOs-0.3.9-mac-applesilicon.dmg` | 100.80 MB | `acd1e36e67b27a3e03f041da13c35ed436bc7bacbdc3cef84fc5a15a76214774` |
| `ClaspOs-0.3.9-mac-intel.dmg` | 105.06 MB | `24f588fc6f21b2be13626ad882f642fe795970077ca67bdb18e54c679375edd2` |
| `ClaspOs-0.3.9-linux.AppImage` | 111.93 MB | `80864cfeb1a6ea6ddfb1f72d4c907272aa3c780f9569b3bb0cc40645632055ae` |
| `ClaspOs-0.3.9-mac-universal.dmg` | 177.87 MB | `c76fd675586de3967cc7b93d3fad3cc70ec2c013f638301186f8c8f325198141` |

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
shasum -a 256 ClaspOs-0.3.9-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.9-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.9-windows.exe SHA256
```
