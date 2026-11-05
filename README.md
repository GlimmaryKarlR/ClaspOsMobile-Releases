# ClaspOS Mobile Official Releases

Public distribution repository for **ClaspOS Mobile** standalone builds and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository only contains official compiled binary distributions and SHA-256 verification hashes.

---

## Latest Release: v0.1.0

### Downloads:

* **macOS (Apple Silicon / Intel)**: `ClaspMobile-0.1.0-mac.zip` (or .dmg)
* **Android (PWA / APK)**: `ClaspMobile-0.1.0-android.zip` (installable via Chrome "Add to Home Screen" or sideload APK)
* **Web (PWA)**: `ClaspMobile-0.1.0-web.zip` (serve the `dist/` folder over HTTPS)

---

### Verified SHA-256 Checksums (v0.1.0)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.1.0-mac.zip` | TBD | TBD |
| `ClaspMobile-0.1.0-android.zip` | TBD | TBD |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

To verify your downloaded binary matches the official build byte-for-byte before running:

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.1.0-mac.zip
sha256sum -c SHA256SUMS.txt
```

### Windows (PowerShell)
```powershell
Get-FileHash .\ClaspMobile-0.1.0-android.zip -Algorithm SHA256
```
