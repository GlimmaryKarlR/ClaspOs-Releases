# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.9

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.9-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.9/ClaspOs-0.5.9-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.9-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.9/ClaspOs-0.5.9-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.9-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.9/ClaspOs-0.5.9-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.9-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.9/ClaspOs-0.5.9-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.9-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.9/ClaspOs-0.5.9-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.9)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.9-windows.exe` | 89.29 MB | `68c3b5ab71d72b74a5299566c0400abc07df857a0edb183679031d17046aaae8` |
| `ClaspOs-0.5.9-mac-applesilicon.dmg` | 102.85 MB | `8d48dd8eb4dbc1672765a7328fdb3966f06a45b91f7e74c845540ef8b8231c0c` |
| `ClaspOs-0.5.9-mac-intel.dmg` | 107.05 MB | `ead56d46f70650cbadab118c92ba8e612a8da94ff0de2436f2b46f8e6a13f850` |
| `ClaspOs-0.5.9-linux.AppImage` | 114.04 MB | `a379e4c5efdf5fccd2b45a964f9804a5ae6f5ba452b6d841cad6f9dfdb42f331` |
| `ClaspOs-0.5.9-mac-universal.dmg` | 179.96 MB | `849ca93e1a82e8cbd617847a3f341909838d3a34e7da0cfbda6c5727be1c2668` |

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
shasum -a 256 ClaspOs-0.5.9-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.9-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.9-windows.exe SHA256
```
