# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.6

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.6-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.6/ClaspOs-0.5.6-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.6-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.6/ClaspOs-0.5.6-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.6-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.6/ClaspOs-0.5.6-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.6-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.6/ClaspOs-0.5.6-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.6-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.6/ClaspOs-0.5.6-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.6)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.6-windows.exe` | 88.23 MB | `78fdc870aa8470c7521fa0e407321dc767bada4cb24fb4a1654a43d5c1628df7` |
| `ClaspOs-0.5.6-mac-applesilicon.dmg` | 101.32 MB | `01a2b027591f2522db74129555ee758c17cc3740044b208097b2fa76858752aa` |
| `ClaspOs-0.5.6-mac-intel.dmg` | 105.56 MB | `df1252c06372261d07e9f023164b31216b51e1da31406436e4336d94854c3919` |
| `ClaspOs-0.5.6-linux.AppImage` | 112.46 MB | `1e9cea53a5e550aa8b6d49afd85b323233f5139950decaee3d8959cc38c9016c` |
| `ClaspOs-0.5.6-mac-universal.dmg` | 178.41 MB | `8d2802843ea8dbae576675e2652c96c0fc257e11a8b1a24b47681bd551d0afd5` |

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
shasum -a 256 ClaspOs-0.5.6-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.6-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.6-windows.exe SHA256
```
