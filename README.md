# AutoLogin

**Version 1.0.1** · macOS 14.2 or later

AutoLogin is a small menu bar app that signs you in to captive Wi-Fi portals (such as Palo Alto Networks portals) automatically, so you don't have to open a browser every time you join the network.

## Download

Get `AutoLogin-1.0.1.dmg` from the [Releases](../../releases/latest) page.

## Install

1. Open the DMG and drag **autologin** into **Applications**.
2. The app is not notarized by Apple, so macOS blocks the first launch. Open the app once, then go to
   **System Settings → Privacy & Security**, scroll down and click **Open Anyway**.
   (On older macOS versions, right-click the app and choose **Open** instead.)
   If it still won't open, run this in Terminal and try again:
   ```
   xattr -cr /Applications/autologin.app
   ```
3. Click the AutoLogin icon in the menu bar and choose **Settings…**.

## Set up

1. Enter your portal **username** and **password**. The password is stored in your macOS login keychain. macOS may ask you to allow access; choose **Always Allow**.
2. Allow **Location access** when asked. macOS requires this before an app can read the Wi-Fi network name (SSID).
3. Tick the **networks that trigger a sign-in**. AutoLogin only acts on the networks you select.
4. Choose a **certificate trust** mode:
   - **Standard**: only certificates macOS already trusts.
   - **Pin a specific certificate** (recommended for self-signed portals): paste the portal certificate's SHA-256 fingerprint. Colons are fine.
   - **Trust any invalid certificate**: less secure. Any certificate presented by the portal host is accepted.
5. Use **Test Sign-in** to check your settings, then **Save**.

Turn on **Open at Login** from the menu bar menu to have it always running.

## How it works

When you join a selected network, AutoLogin checks whether you are online. If you are not, it finds the portal login page and submits your credentials. It retries a few times if the network is still coming up. It never retries a rejected password, so your account can't be locked out.

## Privacy and security

See [PRIVACY.md](PRIVACY.md). In short: credentials stay in your Keychain and are sent only to your portal. Nothing is collected or sent to the author.

## Support

Email [mca.sunildhawan@gmail.com](mailto:mca.sunildhawan@gmail.com).

## Changelog

See [CHANGELOG.md](CHANGELOG.md).

## License

Free to use, not open source. See [LICENSE.txt](LICENSE.txt).
