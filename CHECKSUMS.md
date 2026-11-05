### Verified SHA-256 Checksums (v0.4.5)

Customers can verify the authenticity and integrity of downloaded ClaspOS binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspOs-0.4.5-windows.exe` | 87.86 MB | `0771a644c3ba9383d0848a66813377b4812380df46791f75e7332bb6f46e08c0` |
| `ClaspOs-0.4.5-mac-applesilicon.dmg` | 100.91 MB | `a2539c5dbfa790dbdabb259a0119df5e8535f61c4a22669944d95a830e6cd91e` |
| `ClaspOs-0.4.5-mac-intel.dmg` | 105.10 MB | `2dc469733d70eaf362b72f21e477a98cee19a7e786bda4a3b239cca3d5465f54` |
| `ClaspOs-0.4.5-linux.AppImage` | 112.00 MB | `ecbcb3cf5b052c255569d2b4e34bc7a89d61baf77d9fd5a50e06acca278e0684` |
| `ClaspOs-0.4.5-mac-universal.dmg` | 177.98 MB | `06348bec779dcb08cf4bfeebf4d1bacdb8082a3f7c775172bb90f3490d611d3d` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`
* **Windows (Command Prompt)**: `certutil -hashfile <filename> SHA256`
