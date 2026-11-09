# ClaspOS Mobile Official Releases

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.1.2

> **https://glimmarykarlr.github.io/clasp_mobile/**

### Installation

#### Android
1. Download `ClaspMobile-0.1.2-android.apk` below.
2. On your Android device: "Open"
3. Tap "Install"


#### iOS (PWA)
1. Open https://clasp-mobile.vercel.app/  in SAFARI.
2. Tap the Share button (square with arrow) → "view more" → "Add to Home Screen".
3. The app runs like a native app. 

---

### Verified SHA-256 Checksums (v0.1.2)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.1.2-android.apk` | 4.43 MB | `d73ee9637fa9fc073c3b98ca0945f96704d953756b2c60f5b78c37acbc3b0632` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.1.2-android.apk
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
``` 
