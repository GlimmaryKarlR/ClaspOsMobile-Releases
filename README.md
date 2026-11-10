# ClaspOS Mobile Official Releases

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.1.3

> **https://glimmarykarlr.github.io/clasp_mobile/**

### Installation

#### Android
1. Download `ClaspMobile-0.1.3-android.apk` below.
2. On your Android device: "Open"
3. Tap "Install"


#### iOS (PWA)
1. Open https://clasp-mobile.vercel.app/  in SAFARI.
2. Tap the Share button (square with arrow) → "view more" → "Add to Home Screen".
3. The app runs like a native app. 


---

### Verified SHA-256 Checksums (v0.1.3)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.1.3-android.apk` | 4.43 MB | `1c6efbfea6fab84152f87f97c357c020b7c0fc5f84c71aea3f71b292179ffbdc` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.1.3-android.apk
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
```
