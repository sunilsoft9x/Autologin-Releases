# Changelog

## 1.0.3

- Release tags are now platform-specific: macOS uses `mac-vX.Y.Z`, Windows uses `win-vX.Y.Z`. The in-app updater only looks at `mac-v` releases, so Windows releases never trigger a Mac update.

Updating from 1.0.2: download the DMG and replace the app once (1.0.2 can't read the new tags). From 1.0.3 onward, updates install from inside the app.

## 1.0.2

- Added **Check for Updates…** to the menu. AutoLogin also checks automatically once a week.
- When an update is available, choose **Install and Restart** and AutoLogin downloads, installs and relaunches itself. No manual drag-and-drop needed.
- Added EULA, License, Privacy Policy and Changelog links to the About window.
- Added the EULA (free to use, closed source).

Updating from 1.0.1: download the DMG and replace the app once. From 1.0.2 onward, updates install from inside the app.

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
