# Accora for Mac — Official Releases

This repository distributes official release packages and installation notes for **Accora for Mac**, a native macOS multi-account workspace manager for Zalo Web.

## Latest Release

Download the latest version:
- [GitHub Releases](https://github.com/toanhhg123/accora-releases/releases/latest)

## Installation

1. Download `Accora-<version>-macOS.dmg`.
2. Double-click the `.dmg` file and drag **Accora.app** into the **Applications** folder.

## First Launch (Ad-Hoc Signed / Not Notarized)

Because Accora is currently signed ad-hoc without an Apple Developer ID, macOS Gatekeeper blocks opening on first double-click:

- **Method 1 (Recommended)**: Right-click (Control-click) `Accora.app` in `/Applications` and click **Open**. When the warning dialog appears, click **Open**. Alternatively, open **System Settings → Privacy & Security** and click **Open Anyway**.
- **Method 2 (Terminal)**: Remove the quarantine flag:
  ```sh
  xattr -dr com.apple.quarantine /Applications/Accora.app
  ```

## Privacy

Accora stores all session cookies, accounts, and SQLite databases locally on your Mac within the sandboxed container. No data is synchronized or transmitted to external servers.
