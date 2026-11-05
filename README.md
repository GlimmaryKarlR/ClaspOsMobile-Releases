# ClaspOS Mobile Official Releases

Public distribution repository for **ClaspOS Mobile** standalone builds and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.0.4

### One-Click Install (Recommended)

**Visit the hosted PWA — no download needed:**

> **https://glimmarykarlr.github.io/clasp_mobile/**

Works on Android (Chrome) and iOS (Safari). Tap "Install" / "Add to Home Screen" and it runs full-screen like a native app.

---

### Direct Download Links (GitHub Releases):

* **Android (APK)**: `ClaspMobile-0.0.4-android.apk` — sideload on any Android device
* **Android (PWA Bundle)**: `ClaspMobile-0.0.4-android.zip` — install via Chrome "Add to Home Screen"
* **Web (PWA)**: Serve the `dist/` folder over HTTPS and "Add to Home Screen"

---

### Installation

#### Android (APK — Recommended)
1. Download `ClaspMobile-0.0.4-android.apk` from the GitHub Release.
2. On your Android device: Settings → Security → enable "Install from unknown sources" (or "Allow from this source" for your browser).
3. Open the downloaded APK file → tap "Install".
4. The app installs to your app drawer and runs like a native app.

#### Android (PWA — No download needed)
1. Open **https://glimmarykarlr.github.io/clasp_mobile/** in Chrome on your Android device.
2. Tap the menu (three dots) → "Install app" / "Add to Home Screen".
3. The app installs to your home screen and runs full-screen.

#### iOS (PWA — Recommended, no Apple Developer account needed)
1. Open **https://glimmarykarlr.github.io/clasp_mobile/** in Safari.
2. Tap the Share button (square with arrow) → "Add to Home Screen".
3. The app runs full-screen like a native app. No download or signing needed.

---

### Verified SHA-256 Checksums (v0.0.4)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.0.4-android.apk` | 3.64 MB | `dac109d727ea8dc4a2029babed40348c9b3c58e22173467bdc81d28888c98766` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.0.4-mac-arm64.dmg
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
```
