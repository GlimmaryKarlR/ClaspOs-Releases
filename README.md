# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.5/ClaspOs-0.5.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.5-windows.exe` | 88.06 MB | `0a0caf883552eaf6c280b043b9e73b8d476968954b48f2ef3ba82415eaa429ab` |
| `ClaspOs-0.5.5-mac-applesilicon.dmg` | 101.09 MB | `ba6ebed014d53af5a1e11bab3305abb38751f1308ed19199a83f7fe040576658` |
| `ClaspOs-0.5.5-mac-intel.dmg` | 105.35 MB | `bd0c55815d4936b558cfe343f0d66eb367a9caa0121de83c9300fee466e1ace2` |
| `ClaspOs-0.5.5-linux.AppImage` | 112.23 MB | `39cc74e44be553b4efd22cd0a7a1bf7a20066ea65866586a7cccec6979ec7f3b` |
| `ClaspOs-0.5.5-mac-universal.dmg` | 178.16 MB | `7c3c131b6fee6771a2bf17f848847e50cb97715bc979c06b868cd53096cf603b` |

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
shasum -a 256 ClaspOs-0.5.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.5-windows.exe SHA256
```
