# Beam Wallet Downloads JSON Structure

The JSON structure contains information about the Beam wallet downloads for various platforms, including Windows, Linux, macOS, Android, iOS, and Chrome. Each platform has its version, date, download links, and checksums for verification purposes.

## Windows

- `version`: The Windows wallet version.
- `date`: The release date of the Windows wallet in Unix timestamp format.
- `links`: Download links for the Windows wallet, CLI, and node.
  - `wallet`: The direct link to the Windows wallet executable.
  - `cli`: The direct link to the Windows wallet CLI archive.
  - `node`: The direct link to the Windows node archive.
- `checksums`: Checksums for the wallet, CLI, and node downloads.
  - `wallet`: The SHA256 checksum for the Windows wallet.
  - `cli`: The SHA256 checksum for the Windows wallet CLI.
  - `node`: The SHA256 checksum for the Windows node.

## Linux

- `version`: The Linux wallet version.
- `date`: The release date of the Linux wallet in Unix timestamp format.
- `links`: Download links for the Linux wallet, CLI, and node.
  - `wallet`: The direct link to the Linux wallet archive.
  - `cli`: The direct link to the Linux wallet CLI archive.
  - `node`: The direct link to the Linux node archive.
- `checksums`: Checksums for the wallet, CLI, and node downloads.
  - `wallet`: The SHA256 checksum for the Linux wallet.
  - `cli`: The SHA256 checksum for the Linux wallet CLI.
  - `node`: The SHA256 checksum for the Linux node.

## macOS

- `version`: The macOS wallet version.
- `date`: The release date of the macOS wallet in Unix timestamp format.
- `links`: Download links for the macOS wallet, CLI, and node.
  - `wallet`: The direct link to the macOS wallet disk image.
  - `cli`: The direct link to the macOS wallet CLI archive.
  - `node`: The direct link to the macOS node archive.
- `checksums`: Checksums for the wallet, CLI, and node downloads.
  - `wallet`: The SHA256 checksum for the macOS wallet.
  - `cli`: The SHA256 checksum for the macOS wallet CLI.
  - `node`: The SHA256 checksum for the macOS node.

## Android

- `version`: The Android wallet version.
- `date`: The release date of the Android wallet in Unix timestamp format.
- `links`: Download links for the Android wallet.
  - `wallet`: The direct link to the Android wallet APK.
- `checksums`: Checksums for the wallet download.
  - `wallet`: The SHA256 checksum for the Android wallet.

## iOS

- `links`: Download links for the iOS wallet.
  - `store`: The App Store link for the iOS wallet.
- `checksums`: An empty object, as checksums are not provided for iOS.

## Chrome

- `links`: Download links for the Chrome web wallet.
  - `store`: The Chrome Web Store link for the Chrome web wallet.
- `checksums`: An empty object, as checksums are not provided for Chrome.

# Example

```json
{
  "windows": {
    "version": STRING, // The version number of the software.
    "date": INTEGER, // The release date as a UNIX timestamp.
    "links": {
      "wallet": STRING, // Download link for the Beam Wallet application.
      "cli": STRING, // Download link for the Beam Wallet CLI.
      "node": STRING // Download link for the Beam Node.
    },
    "checksums": {
      "wallet": STRING, // Checksum for the Beam Wallet application.
      "cli": STRING, // Checksum for the Beam Wallet CLI.
      "node": STRING // Checksum for the Beam Node.
    }
  },
  "linux": {
    "version": STRING, // The version number of the software.
    "date": INTEGER, // The release date as a UNIX timestamp.
    "links": {
      "wallet": STRING, // Download link for the Beam Wallet application.
      "cli": STRING, // Download link for the Beam Wallet CLI.
      "node": STRING // Download link for the Beam Node.
    },
    "checksums": {
      "wallet": STRING, // Checksum for the Beam Wallet application.
      "cli": STRING, // Checksum for the Beam Wallet CLI.
      "node": STRING // Checksum for the Beam Node.
    }
  },
  "macos": {
    "version": STRING, // The version number of the software.
    "date": INTEGER, // The release date as a UNIX timestamp.
    "links": {
      "wallet": STRING, // Download link for the Beam Wallet application.
      "cli": STRING, // Download link for the Beam Wallet CLI.
      "node": STRING // Download link for the Beam Node.
    },
    "checksums": {
      "wallet": STRING, // Checksum for the Beam Wallet application.
      "cli": STRING, // Checksum for the Beam Wallet CLI.
      "node": STRING // Checksum for the Beam Node.
    }
  },
  "android": {
    "version": STRING, // The version number of the software.
    "date": INTEGER, // The release date as a UNIX timestamp.
    "links": {
      "wallet": STRING // Download link for the Beam Wallet APK.
    },
    "checksums": {
      "wallet": STRING // Checksum for the Beam Wallet APK.
    }
  },
  "ios": {
    "links": {
      "store": STRING // Link to the Beam Wallet on the Apple App Store.
    },
    "checksums": {}
  },
  "chrome": {
    "links": {
      "store": STRING // Link to the Beam Web Wallet on the Chrome Web Store.
    },
    "checksums": {}
  }
}
```
