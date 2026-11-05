# ClaspOS Mobile Official Releases

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.0.6

> **https://glimmarykarlr.github.io/clasp_mobile/**

### Installation

#### Android
1. Download `ClaspMobile-0.0.6-android.apk` from the GitHub Release.
2. On your Android device: Settings → Security → enable "Install from unknown sources" (or "Allow from this source" for your browser).
3. Open the downloaded APK file → tap "Install".
4. The app installs to your app drawer and runs like a native app.

#### iOS (PWA)
1. Open **https://glimmarykarlr.github.io/clasp_mobile/** in SAFARI.
2. Tap the Share button (square with arrow) → "Add to Home Screen".
3. The app runs full-screen like a native app. No download or signing needed.

---

### Verified SHA-256 Checksums (v0.0.6)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.0.6-android.apk` | 3.67 MB | `485995833554aefa8426ae87c1e0225be6a0e9a2ec172f61cdd8fd3d0db7f4a4` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.0.6-android.apk
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
```
