# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.3

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.3-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.3/ClaspOs-0.4.3-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.3-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.3/ClaspOs-0.4.3-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.3-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.3/ClaspOs-0.4.3-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.3-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.3/ClaspOs-0.4.3-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.3-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.3/ClaspOs-0.4.3-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.3)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.3-windows.exe` | 87.86 MB | `42cd829391295eaf4e8c0c26863be3a5fdc94cb92e8540e05863d3ac612f56b6` |
| `ClaspOs-0.4.3-mac-applesilicon.dmg` | 100.89 MB | `c8ee79c5b988b12609f17b97c91a5804d4e7680f173baf6cc3c5a6417f233629` |
| `ClaspOs-0.4.3-mac-intel.dmg` | 105.10 MB | `018609fef4d08427ea2bf24f8137abe19de2723a37c3e7ea96b4b513addfbdd5` |
| `ClaspOs-0.4.3-linux.AppImage` | 112.00 MB | `39152665a03d41ce5df5892ca3b7ff38c12473b23e6893ff6d07cebc3036b862` |
| `ClaspOs-0.4.3-mac-universal.dmg` | 178.00 MB | `02d7cde9c391af84d7c49e157729faa65249d85dc9a0a537a847d1929bac823f` |

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
shasum -a 256 ClaspOs-0.4.3-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.3-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.3-windows.exe SHA256
```
