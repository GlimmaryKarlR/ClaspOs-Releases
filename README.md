# ClaspOS Official Standalone Releases

Public distribution repository for **ClaspOS** standalone workstation binaries and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS source code is proprietary and private. This repository only contains official compiled binary distributions and SHA-256 verification hashes for customers.

---

## Latest Release: v0.2.0

### Downloads:

* **Windows 10 / 11**: [`ClaspOs-0.2.0-windows.exe`](./ClaspOs-0.2.0-windows.exe)
* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: [`ClaspOs-0.2.0-mac-applesilicon.dmg`](./ClaspOs-0.2.0-mac-applesilicon.dmg)
* **macOS (Intel Core x86_64)**: [`ClaspOs-0.2.0-mac-intel.dmg`](./ClaspOs-0.2.0-mac-intel.dmg)
* **Linux (Ubuntu, Debian, Fedora, Arch)**: [`ClaspOs-0.2.0-linux.AppImage`](./ClaspOs-0.2.0-linux.AppImage)

---

### Verified SHA-256 Checksums (v0.2.0)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.2.0-windows.exe` | 83.35 MB | `a73a87519be72dd14e086b7528b0deae99c1712803939c4fbd90c3d48dc117b7` |
| `ClaspOs-0.2.0-mac-applesilicon.dmg` | 95.28 MB | `17b1a1c0ea9b1606a014ffbe03b170fb98a8a6a3adbefaa0fbc387b3e0aa8c12` |
| `ClaspOs-0.2.0-mac-intel.dmg` | 99.53 MB | `f8087601f27f0e3d1a6c98216fabc48ae08d4178b61432f8c0d1bd212b756142` |
| `ClaspOs-0.2.0-linux.AppImage` | 106.37 MB | `d1d2621d43c812a99c9acd70c89269ab597f391f22fcd87c4fde35d9a3cf0559` |
| `ClaspOs-0.2.0-mac-universal.dmg` | 172.37 MB | `f154c7c9c0767b9190f55699c7c43dcdf4601564eb7c37d08b1977e73babded6` |

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
shasum -a 256 ClaspOs-0.2.0-mac-applesilicon.dmg

# Or verify entire SHA256SUMS file:
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspOs-0.2.0-windows.exe -Algorithm SHA256
```

### Windows (Command Prompt)
```cmd
certutil -hashfile ClaspOs-0.2.0-windows.exe SHA256
```
