# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.7.0

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.7.0-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.7.0/ClaspOs-0.7.0-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.7.0-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.7.0/ClaspOs-0.7.0-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.7.0-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.7.0/ClaspOs-0.7.0-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.7.0-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.7.0/ClaspOs-0.7.0-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.7.0-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.7.0/ClaspOs-0.7.0-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.7.0)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.7.0-windows.exe` | 90.11 MB | `17ee4a8c26ac46d522ee18ac1ada3021f10a5ba707b24c1552a1f71b65c085de` |
| `ClaspOs-0.7.0-mac-applesilicon.dmg` | 104.07 MB | `78418b7d678a5ce6e26eafa7fcf489838fae11e704f05c5df699e4655778478a` |
| `ClaspOs-0.7.0-mac-intel.dmg` | 108.33 MB | `8567240c2dfc09f559d6222928363291181cdd2e098192033d12a20915b991cd` |
| `ClaspOs-0.7.0-linux.AppImage` | 115.35 MB | `4f35177b08618ca8e2b5b43f8231958a6b2e535b650c2121853cedb0f76cad11` |
| `ClaspOs-0.7.0-mac-universal.dmg` | 181.13 MB | `e4dfd20fa5b4c2794088e3c50deac6361b6701323590bbe7ee039d5cfb7d1ad5` |

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
shasum -a 256 ClaspOs-0.7.0-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.7.0-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.7.0-windows.exe SHA256
```
