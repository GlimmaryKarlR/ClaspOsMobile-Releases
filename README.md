# ClaspOS Mobile Official Releases

Public distribution repository for **ClaspOS Mobile** standalone builds and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.0.2

### One-Click Install (Recommended)

**Visit the hosted PWA — no download needed:**

> **https://glimmarykarlr.github.io/clasp_mobile/**

Works on Android (Chrome) and iOS (Safari). Tap "Install" / "Add to Home Screen" and it runs full-screen like a native app.

---

### Direct Download Links (GitHub Releases):

* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: `ClaspMobile-0.0.2-mac-arm64.dmg` / `.zip`
* **macOS (Intel Core x86_64)**: `ClaspMobile-0.0.2-mac-x64.dmg` / `.zip`
* **macOS (Universal - Both M-Series & Intel)**: `ClaspMobile-0.0.2-mac-universal.dmg` / `.zip`
* **Android (PWA / Web Bundle)**: `ClaspMobile-0.0.2-android.zip` — or use the one-click install above

---

### Installation

#### One-Click (Android + iOS — Recommended)
1. Open **https://glimmarykarlr.github.io/clasp_mobile/** in your phone's browser.
2. **Android (Chrome)**: Tap the menu (three dots) → "Install app" / "Add to Home Screen".
3. **iOS (Safari)**: Tap Share (square with arrow) → "Add to Home Screen".
4. The app installs to your home screen and runs full-screen. No download needed.

#### macOS (Desktop App)
1. Download the `.dmg` for your architecture (Apple Silicon or Intel).
2. Open the DMG and drag **ClaspMobile** into your Applications folder.
3. Launch ClaspMobile from Applications.
4. On first launch, scan the QR code in the desktop ClaspOS app (Pro tab → Pair Mobile Device) to connect.

#### Android (Manual / Offline)
1. Download `ClaspMobile-0.0.2-android.zip` and extract.
2. Serve the folder: `npx serve dist/` or `python3 -m http.server 8080`
3. Open `http://<your-pc-ip>:8080` in Chrome on your Android device (same Wi-Fi).
4. Chrome will show "Install app" → tap it.

#### iOS (Manual / Offline)
1. Serve the extracted web bundle over HTTPS or localhost.
2. Open in Safari → Share → "Add to Home Screen".

---

### Verified SHA-256 Checksums (v0.0.2)

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspMobile-0.0.2-arm64-mac.zip` | 93.45 MB | `4231dab468f935f93d08c581dad630b7c0242849dd9456f09fdb9f84c28a7604` |
| `ClaspMobile-0.0.2-mac.zip` | 97.73 MB | `507cc5c5805c44f791681a1d43567a4f1c6059c996885b282df91f0071e2a4fc` |
| `ClaspMobile-0.0.2-android.zip` | 0.13 MB | `6a38bf22fee134c32d13cf612e67f6c8dd223a975e3341905c4c65ae8b1c0c19` |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`

---

## Integrity Verification Guide

### macOS / Linux
```bash
shasum -a 256 ClaspMobile-0.0.2-mac-arm64.dmg
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
```
