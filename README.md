# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.3.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.3.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.3.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.3.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.3.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.3.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.3.5/ClaspOs-0.3.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.3.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.3.5-windows.exe` | 87.71 MB | `51bf650b63d81d1e1ec5de0bdf835fc557af1743d7bcc3569497decc75e5789e` |
| `ClaspOs-0.3.5-mac-applesilicon.dmg` | 100.68 MB | `d9bf239666dc4c68eb25c4583bf9cc59996f7e93b33f13fbdb78172da335e846` |
| `ClaspOs-0.3.5-mac-intel.dmg` | 104.96 MB | `8edd67397d0a44b35fe4ae2cac87d44d62a53ed8cc73d21e6fb2ffb35f43e07f` |
| `ClaspOs-0.3.5-linux.AppImage` | 111.80 MB | `9a5ff7b41996c104e0d2273d84f1ee58b7e03c54bf39ca6e94d7f01d465b5677` |
| `ClaspOs-0.3.5-mac-universal.dmg` | 177.77 MB | `6526c74699945b62026082d9c229be1517b7dac8ad4b7526e2d0060c08f29e33` |

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
shasum -a 256 ClaspOs-0.3.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.3.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.3.5-windows.exe SHA256
```
