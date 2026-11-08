# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.0

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.0-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.0/ClaspOs-0.5.0-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.0-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.0/ClaspOs-0.5.0-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.0-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.0/ClaspOs-0.5.0-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.0-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.0/ClaspOs-0.5.0-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.0-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.0/ClaspOs-0.5.0-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.0)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.0-windows.exe` | 87.89 MB | `64a53dba22cd4510449e6c41cc6538854b8010e86b9a923eba13f70eba4356e5` |
| `ClaspOs-0.5.0-mac-applesilicon.dmg` | 100.91 MB | `c38edb19757f08ca63909ed28d797e8ec968746427347e0c80495f88c936c773` |
| `ClaspOs-0.5.0-mac-intel.dmg` | 105.14 MB | `c5ef0bfdec4cdfc4185d3bd43e143a5a0f3279484fe179eb702aab7c3bedb824` |
| `ClaspOs-0.5.0-linux.AppImage` | 112.04 MB | `9364f87b6b586018215f212750d7af484794080f164923259ae63b0dbecc94d1` |
| `ClaspOs-0.5.0-mac-universal.dmg` | 178.00 MB | `5d19b51384f8a063478bbb9732055fe8e83e1d61f47aa95f2157eab5b1ee8948` |

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
shasum -a 256 ClaspOs-0.5.0-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.0-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.0-windows.exe SHA256
```
