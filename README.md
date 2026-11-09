# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.1

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.1-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.1/ClaspOs-0.5.1-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.1-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.1/ClaspOs-0.5.1-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.1-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.1/ClaspOs-0.5.1-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.1-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.1/ClaspOs-0.5.1-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.1-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.1/ClaspOs-0.5.1-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.1)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.1-windows.exe` | 87.96 MB | `a5dccc5fc7135a651093f8cf2908835fa82cfa666244f4a0ad524e95a038a9b3` |
| `ClaspOs-0.5.1-mac-applesilicon.dmg` | 100.99 MB | `d74b6c2c21a944b8984e7276fec4582652de33ac249088eb50fe4b511dfc1766` |
| `ClaspOs-0.5.1-mac-intel.dmg` | 105.22 MB | `11a37520425000d5066c18e9c1e9ab6fb9374c9dc64875c8672dcd4dcef050de` |
| `ClaspOs-0.5.1-linux.AppImage` | 112.13 MB | `8279fdd68026927034316defa8feb812e48134c988f00e6e6c3fbb9701daef33` |
| `ClaspOs-0.5.1-mac-universal.dmg` | 178.09 MB | `155824d62fcc48c70e8f6028456b30c2ac784b7f424492b3aa5328ce7529c418` |

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
shasum -a 256 ClaspOs-0.5.1-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.1-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.1-windows.exe SHA256
```
