# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.2.5

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.2.5-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.5/ClaspOs-0.2.5-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.2.5-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.5/ClaspOs-0.2.5-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.2.5-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.5/ClaspOs-0.2.5-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.2.5-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.5/ClaspOs-0.2.5-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.2.5-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.2.5/ClaspOs-0.2.5-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.2.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.2.5-windows.exe` | 83.63 MB | `cba5e9908b69762701d456aa939f11e3264dec903cd11fa29c597b2e44e7a823` |
| `ClaspOs-0.2.5-mac-applesilicon.dmg` | 95.65 MB | `95e8d9afd8357eee2f8f0297cdca4718e0b9c47d18ada747ab2f499732458c51` |
| `ClaspOs-0.2.5-mac-intel.dmg` | 99.91 MB | `55a06fdd28413b99baa3eecb01442d5750f1d067ba11024337fe63477fda9791` |
| `ClaspOs-0.2.5-linux.AppImage` | 106.73 MB | `ab3c537c7ffb5799535567fb129bd8089f1752b708765797b42369027e1bc00e` |
| `ClaspOs-0.2.5-mac-universal.dmg` | 172.73 MB | `253d5e193560ab1f51f2b49971c84a4bb4e23de93fffcbd5bdc3c191c43cf09a` |

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
shasum -a 256 ClaspOs-0.2.5-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.2.5-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.2.5-windows.exe SHA256
```
