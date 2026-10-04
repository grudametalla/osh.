# osh. privacy

[Русский](PRIVACY.md) · **English**

Revision: October 4, 2026.

osh. processes network traffic only as required by the connection features selected by the user.

Telegram Bridge uses a local proxy. Smart Access uses the Android VPN interface to route traffic for selected YouTube and Discord applications.

## What osh. does not do

In the current public beta, osh.:

- has no built-in advertising analytics;
- does not send Telegram message contents to the osh. owner;
- does not send media contents or browsing history to the osh. owner;
- does not upload diagnostic reports automatically.

## Data stored on the device

Settings, technical state and local secrets are stored in the app's private storage.

Telegram/proxy secrets are protected using Android Keystore. Standard Android backup and device transfer are disabled for private app data.

Diagnostics keep a limited number of local reports and remove older data automatically.

## Network requests

The app may connect to GitHub for updates, Telegram/YouTube/Discord endpoints, technical reachability endpoints, and intermediate relay/proxy nodes when required by the selected route.

An intermediate network node can observe normal transport metadata such as connection timing and traffic volume. osh. does not provide Telegram message contents to that node in plaintext.

## Diagnostic reports

A diagnostic export is started only by the user through the Android system share flow. Review a report before sending it to a third party.

## Permissions

osh. uses Internet, network state, foreground service, VPNService, notifications, boot/autostart and APK installer permissions only for documented application functions.

If future versions introduce accounts, paid server-side features or new telemetry, this policy will be updated before those features are enabled publicly.

osh. is not designed to hide a user's identity on the Internet.
