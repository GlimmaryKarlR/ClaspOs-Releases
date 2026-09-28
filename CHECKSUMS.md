### Verified SHA-256 Checksums (v0.2.1)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.2.1-windows.exe` | 83.44 MB | `e4f1cfcb47f2968ca4ac907dec3ed06e3b5d05d19e5bda38c7eb5ce4183f7d6b` |
| `ClaspOs-0.2.1-mac-applesilicon.dmg` | 95.40 MB | `c797af3540f135403dc9f0816969ac3214e564ef2033bcba68f424ad85610621` |
| `ClaspOs-0.2.1-mac-intel.dmg` | 99.66 MB | `fb3e28025fadecc31200b9a25ccf318dc2b7abe63c9a927deb7fe5c1418a273d` |
| `ClaspOs-0.2.1-linux.AppImage` | 106.47 MB | `48368ef1e9085c8ce674ba0e60cd27c300b2715452e12097037a7bba6e5c7fbb` |
| `ClaspOs-0.2.1-mac-universal.dmg` | 172.48 MB | `eceff7114ef6be3d80e64f166c44f9b2bab949dac47762c4699c5aacf0a38d69` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`
* **Windows (Command Prompt)**: `certutil -hashfile <filename> SHA256`
