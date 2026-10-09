# Changelog

## 1.0.1

- Fixed the app not launching on other Macs. The 1.0 build was tied to the developer's Mac.
- The password is now stored in the macOS login keychain. Re-enter your password once after installing.
- Added an app icon.
- Updated install instructions for macOS 15 and later.

## 1.0

Initial release.

- Menu bar app that signs in to captive Wi-Fi portals automatically.
- Choose which Wi-Fi networks trigger a sign-in.
- Automatic portal detection, with an optional manual portal URL.
- Certificate trust modes: standard, pinned SHA-256 fingerprint, or trust any invalid certificate.
- Password stored in the macOS Keychain.
- Automatic retries, and no retry after a rejected password.
- Test Sign-in button, Open at Login option, and light/dark appearance setting.
