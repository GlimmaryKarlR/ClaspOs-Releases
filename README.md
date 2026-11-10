# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.5.3

### Direct Download Links (GitHub Releases):

* **Windows 10 / 11 (x64)**: [`ClaspOs-0.5.3-windows.exe`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.3/ClaspOs-0.5.3-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.5.3-mac-applesilicon.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.3/ClaspOs-0.5.3-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.5.3-mac-intel.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.3/ClaspOs-0.5.3-mac-intel.dmg)
* **macOS (Universal - Both M-Series & Intel)**: [`ClaspOs-0.5.3-mac-universal.dmg`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.3/ClaspOs-0.5.3-mac-universal.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.5.3-linux.AppImage`](https://github.com/GlimmaryKarlR/ClaspOs-Releases/releases/download/v0.5.3/ClaspOs-0.5.3-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.5.3)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.5.3-windows.exe` | 87.95 MB | `08ba2fe11d84e887ae69052673061863ebcf47b0a6e03220b14dc8efabb65eb3` |
| `ClaspOs-0.5.3-mac-applesilicon.dmg` | 101.02 MB | `a48561b2a89e876bfd5541a173b55af1bfa3bc02caed194cf73bb369f94f27e7` |
| `ClaspOs-0.5.3-mac-intel.dmg` | 105.21 MB | `a87f18a51a5eed80fae664f6422b455ff6eba29dd8218d469c72c0f6bc2f9050` |
| `ClaspOs-0.5.3-linux.AppImage` | 112.11 MB | `fbd56eb5fb58597baf95c943f3925e1ccec1fec67b1f056f28c7fda62caeced9` |
| `ClaspOs-0.5.3-mac-universal.dmg` | 178.08 MB | `909d17d1e1b95b34c023c0383ca5e7dd0d38e3b15fa410b676461a7438387be1` |

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
shasum -a 256 ClaspOs-0.5.3-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.5.3-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.5.3-windows.exe SHA256
```
