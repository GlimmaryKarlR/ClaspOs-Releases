# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.4.9

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.4.9-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.9/ClaspOs-0.4.9-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.4.9-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.9/ClaspOs-0.4.9-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.4.9-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.9/ClaspOs-0.4.9-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.4.9-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.9/ClaspOs-0.4.9-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.4.9-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.4.9/ClaspOs-0.4.9-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.4.9)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.9-windows.exe` | 87.89 MB | `e9044804fb8b9e1d68690690741cba7ef9d52454fca4bb6423aa1692ede6e345` |
| `ClaspOs-0.4.9-mac-applesilicon.dmg` | 100.91 MB | `1fa4e05d4525d96f339c759cb3ecdcbc7e1378d0d2d3c315a7f07926cfafe1e9` |
| `ClaspOs-0.4.9-mac-intel.dmg` | 105.15 MB | `fdc5abc14bacb9b107bc74d0a7fe019747b45590312ef17b176078c8d140813e` |
| `ClaspOs-0.4.9-linux.AppImage` | 112.03 MB | `8a26fe1f30fc9c4f67845f1801f111950884fd8fd467b2061d6d5ee2790f46c0` |
| `ClaspOs-0.4.9-mac-universal.dmg` | 178.00 MB | `ff1b3d28b95907df43195ef3fd3fd3715764592f8e495b7a7fbcc6d8505fa066` |

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
shasum -a 256 ClaspOs-0.4.9-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.4.9-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.4.9-windows.exe SHA256
```
