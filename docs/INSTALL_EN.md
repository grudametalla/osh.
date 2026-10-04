# Installing osh.

[Русский](INSTALL.md) · **English**

## 1. Download an APK

Use only the [official Releases](https://github.com/grudametalla/osh./releases).

- `osh-<version>-arm64-v8a.apk` is recommended for modern Android phones.
- `osh-<version>-universal.apk` is the universal ARM64 + x86_64 build.
- `SHA256SUMS.txt` contains release file checksums.
- `RELEASE-METADATA.json` contains technical release metadata.

Minimum Android version: **8.0 (API 26)**.

## 2. Install

Open the downloaded APK and confirm installation in the Android system installer. osh. shows the quick setup on first launch.

Android may separately request VPN permission when YouTube or Discord is enabled.

## 3. Verify the checksum

Windows PowerShell:

```powershell
Get-FileHash .\osh-0.1.0-beta.1-arm64-v8a.apk -Algorithm SHA256
```

Compare the result with the matching entry in `SHA256SUMS.txt`.

## 4. Verify the APK signature

With Android SDK installed:

```text
apksigner verify --print-certs osh-0.1.0-beta.1-arm64-v8a.apk
```

Official osh. production certificate SHA-256 fingerprint:

`a5327cd2a2c0c48e6805467ae22cc5db83a7fd54c84715d1cc9dc94c5f6c0c9c`

If the fingerprint differs, do not install the file as an official osh. build.

## Updates

osh. checks the official GitHub repository for updates. The downloaded APK is verified and then handed to the Android system installer.

There is no silent installation without user confirmation.

Updating over an existing installation requires the same signing certificate and a higher `versionCode`.

## Troubleshooting installation

Check that APK installation is allowed for the app opening the file, enough free storage is available, a build signed with another certificate is not already installed, and an older build is not being installed over a newer one.

For regular problems, use [Issues](https://github.com/grudametalla/osh./issues).
