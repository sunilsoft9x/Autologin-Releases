# Privacy and Security

**Effective with version 1.0.1**

## What AutoLogin stores

- **Username and portal settings:** saved locally on your Mac.
- **Password:** saved in the macOS login keychain, never in plain text.

## What AutoLogin accesses

- **Wi-Fi network name (SSID):** read locally to decide whether to sign in. macOS requires Location permission for this. AutoLogin does not read or store your physical location.

## What AutoLogin sends

- Your credentials are sent only to your captive portal, to sign you in.
- AutoLogin also contacts `captive.apple.com` to check whether you are online.
- **Nothing is sent to the author or any third party.** There is no analytics, tracking or telemetry.

## Certificates

Many captive portals use self-signed certificates. AutoLogin offers:

- **Pin a specific certificate** (recommended): only the certificate with your SHA-256 fingerprint is accepted for the portal host.
- **Trust any invalid certificate**: less secure. Anyone able to impersonate the portal address could capture your credentials. Use it only on networks you trust.

Certificate trust applies only to the portal host. Other hosts use normal system validation.

## Contact

[mca.sunildhawan@gmail.com](mailto:mca.sunildhawan@gmail.com)
