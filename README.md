# ClaspOS Mobile Official Releases

Public distribution repository for **ClaspOS Mobile** standalone builds and verified cryptographic checksums.

> **Source Code Notice**: ClaspOS Mobile source code is proprietary and private. This repository contains official release documentation, SHA-256 verification hashes, and direct download links to GitHub Release assets.

---

## Latest Release: v0.0.2

### Direct Download Links (GitHub Releases):

* **macOS (Apple Silicon M1 / M2 / M3 / M4)**: `ClaspChat-0.0.2-mac-arm64.dmg` / `.zip`
* **macOS (Intel Core x86_64)**: `ClaspChat-0.0.2-mac-x64.dmg` / `.zip`
* **macOS (Universal - Both M-Series & Intel)**: `ClaspChat-0.0.2-mac-universal.dmg` / `.zip`
* **Android (PWA / Web Bundle)**: `ClaspMobile-0.0.2-android.zip` — install via Chrome "Add to Home Screen" or convert to APK via TWA/Bubblewrap
* **Web (PWA)**: Serve the `dist/` folder over HTTPS and "Add to Home Screen"

---

### Installation

#### macOS
1. Download the `.dmg` for your architecture (Apple Silicon or Intel).
2. Open the DMG and drag **ClaspChat** into your Applications folder.
3. Launch ClaspChat from Applications.
4. On first launch, scan the QR code in the desktop ClaspOS app (Pro tab → Pair Mobile Device) to connect.

#### Android
1. Download `ClaspMobile-0.0.2-android.zip` and extract, or visit the hosted PWA URL.
2. Open in Chrome → tap the menu → **"Add to Home Screen"** / **"Install app"**.
3. The app runs full-screen like a native app.
4. On first launch, tap "Scan QR" in the Clasp Chat tab and point your camera at the desktop's QR code.

#### iOS
1. Open the hosted PWA URL in Safari.
2. Tap the Share button → **"Add to Home Screen"**.
3. The app runs full-screen like a native app.

---

### Verified SHA-256 Checksums (v0.0.2)

Customers can verify the authenticity and integrity of downloaded ClaspOS Mobile binaries before running them:

| Platform / Binary | Size | SHA-256 Checksum |
| :--- | :--- | :--- |
| `ClaspChat-0.0.2-mac-arm64.dmg` | TBD | TBD |
| `ClaspChat-0.0.2-mac-x64.dmg` | TBD | TBD |
| `ClaspChat-0.0.2-mac-universal.dmg` | TBD | TBD |
| `ClaspMobile-0.0.2-android.zip` | TBD | TBD |

#### How to Verify Locally:
* **macOS / Linux**: `shasum -a 256 <filename>` (or `sha256sum -c SHA256SUMS.txt`)
* **Windows (PowerShell)**: `Get-FileHash <filename> -Algorithm SHA256`
* **Windows (Command Prompt)**: `certutil -hashfile <filename> SHA256`

---

## Integrity Verification Guide

To verify your downloaded binary matches the official build byte-for-byte before running:

### macOS / Linux
```bash
shasum -a 256 ClaspChat-0.0.2-mac-arm64.dmg
sha256sum -c SHA256SUMS.txt
```

### Android (after extracting zip)
```bash
sha256sum -c SHA256SUMS.txt
```
EOF
echo "written"