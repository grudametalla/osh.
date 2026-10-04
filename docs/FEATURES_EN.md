# osh. features

[Русский](FEATURES.md) · **English**

## Telegram Bridge

osh. runs a local proxy on the device and passes ready-to-use parameters to Telegram. Users do not need to copy proxy addresses and ports manually.

The bridge is independent from Android VPN, so Telegram can be used without Smart Access.

## Smart Access

Smart Access is designed for YouTube and Discord.

- a single Android VPN is shared by both apps;
- only selected application traffic is routed through it;
- all other apps continue to use the normal Internet connection;
- routes are selected automatically;
- when a route fails, osh. attempts to recover it without restarting the entire app.

## Connection modes

**Auto** is intended for normal use: osh. selects routes and handles recovery automatically.

**Manual** provides more control and is useful when troubleshooting unusual networks.

## Network changes and recovery

osh. tracks Wi-Fi/LTE changes and the state of active routes. After temporary network failures it retries the connection while trying to avoid disturbing services that are still working.

## Connection check

The **Check** section runs diagnostics and helps identify where a connection problem occurred. Diagnostic reports are exported only when the user explicitly chooses to share them.

## System integration

- optional autostart after reboot;
- Android Quick Settings tile;
- foreground service notification;
- updates through the Android system installer;
- downloaded APK signature verification before update.

## Privacy

osh. has no built-in advertising analytics and does not send message contents or browsing history to the app owner.

Settings and technical state are stored locally. See [PRIVACY_EN.md](PRIVACY_EN.md).

## Public beta limitations

- Telegram, YouTube and Discord availability depends on the current network;
- Android allows only one active VPNService, so Smart Access can conflict with another VPN;
- osh. is not intended to anonymize all device traffic;
- connection routes and methods may change between releases.

Current builds and release notes are published in [Releases](https://github.com/grudametalla/osh./releases).
