# ClaspOS Mobile Official Releases

Public distribution repository for **ClaspOS Mobile** standalone builds and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.0.3

### One-Click Install (Recommended)

**Visit the hosted PWA — no download needed:**

> **https://glimmarykarlr.github.io/clasp_mobile/**

Works on Android (Chrome) and iOS (Safari). Tap "Install" / "Add to Home Screen" and it runs full-screen like a native app.

---

### Direct Download Links (GitHub Releases):

* **Android (APK)**: `ClaspMobile-0.0.3-android.apk` — sideload on any Android device
* **Android (PWA Bundle)**: `ClaspMobile-0.0.3-android.zip` — install via Chrome "Add to Home Screen"
* **iOS (.ipa)**: `ClaspMobile-0.0.3.ipa` — OTA install via manifest.plist (requires Apple Developer account)

---

### Installation

#### Android (APK — Recommended)
1. Download `ClaspMobile-0.0.3-android.apk` from the GitHub Release.
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

#### iOS (OTA .ipa — requires Apple Developer account)
1. Build the .ipa using Xcode or GitHub Actions (macos-latest runner) with an Ad-Hoc provisioning profile.
2. Upload the .ipa to a GitHub Release.
3. Update `manifest.plist` with the .ipa download URL and bundle version.
4. Commit `manifest.plist` to this repo and get the raw URL.
5. Open this link on a registered iOS device:
   `itms-services://?action=download-manifest&url=YOUR_RAW_PLIST_URL`
6. iOS will prompt to install the app over-the-air.

> **Note:** iOS OTA distribution requires an Apple Developer account ($99/yr) and an Ad-Hoc or Enterprise provisioning profile. Devices must be registered in the provisioning profile. For broader distribution, use TestFlight or the App Store.

---

### Verified SHA-256 Checksums (v0.0.3)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.0.3-android.apk` | 4.12 MB | `6babc22a86aa9237898b08ee9aa1b14a97c3491f373cbe089f56a6a47318ebf6` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.0.3-mac-arm64.dmg
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
```
