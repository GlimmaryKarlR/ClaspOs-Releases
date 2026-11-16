# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.8

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.8-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.8/ClaspOs-0.5.8-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.8-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.8/ClaspOs-0.5.8-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.8-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.8/ClaspOs-0.5.8-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.8-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.8/ClaspOs-0.5.8-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.8-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.8/ClaspOs-0.5.8-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.8)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.8-windows.exe` | 89.02 MB | `bccd831ecf189a8c157ee26772de6a9555be75f324b13b3a660b67d397eb0c08` |
| `ClaspOs-0.5.8-mac-applesilicon.dmg` | 102.37 MB | `1bebb626cd27ba821bfd5992ad27945df0dc5da922e73a19d995a54a29c65fe9` |
| `ClaspOs-0.5.8-mac-intel.dmg` | 106.56 MB | `59bf5b0b44e0b4a08553be243ff301567aa9fc3e5cfd9b83528ac88c2088bc46` |
| `ClaspOs-0.5.8-linux.AppImage` | 113.52 MB | `90fc560f917f2b2716e110d78da6f093320f01b93694513f4ea2eda8100342d6` |
| `ClaspOs-0.5.8-mac-universal.dmg` | 179.46 MB | `ed46f7e1f3bdae3a40303680d30dcefc97257f34557df5b6dd3e8bfae896d915` |

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
shasum -a 256 ClaspOs-0.5.8-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.8-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.8-windows.exe SHA256
```
