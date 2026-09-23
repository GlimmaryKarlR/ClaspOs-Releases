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
