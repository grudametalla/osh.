# osh. security

[Русский](SECURITY.md) · **English**

## Verifying an official build

Use APK files only from this repository's [Releases](https://github.com/grudametalla/osh./releases).

Official osh. production certificate SHA-256 fingerprint:

`a5327cd2a2c0c48e6805467ae22cc5db83a7fd54c84715d1cc9dc94c5f6c0c9c`

Step-by-step APK verification is documented in [INSTALL_EN.md](INSTALL_EN.md).

Android verifies the signing certificate when updating an installed application. osh. also verifies the downloaded APK before handing it to the system installer.

Updates are never installed silently.

## Reporting a vulnerability

Use the repository's **Security** tab and Private vulnerability reporting when available.

Do not post vulnerability exploitation details, tokens, keys, passwords, message contents, private diagnostic reports or personal user data in regular Issues.

If GitHub's private reporting form is unavailable, open an Issue only to request a secure communication channel, without technical vulnerability details.

## Fake APKs and impersonation

If a third-party site, account, store or APK claims to be official osh., open a regular Issue with the public URL, file name, SHA-256 and certificate fingerprint when available.

Do not install repackaged builds signed with another certificate.

## Testing boundaries

Test vulnerabilities only on devices and data you own or when you have explicit authorization from the owner.

The proprietary osh. source code is not published in this binary distribution repository.
