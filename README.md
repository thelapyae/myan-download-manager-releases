# Myan - Download Manager

Native download manager for macOS with multipart downloads and browser
integration.

## Download

Download the latest version from the
[Releases](https://github.com/thelapyae/myan-download-manager-releases/releases)
page.

Current beta requirements:

- macOS 14 or later
- Apple Silicon Mac
- Chrome, Arc, or Safari for browser integration

## Install The App

1. Download `Myan-Download-Manager-*-macOS-arm64.zip`.
2. Extract the ZIP.
3. Move **Myan - Download Manager.app** to `/Applications`.
4. Open the app once. This automatically installs the Chrome and Arc native
   messaging connection.

This beta is Developer ID signed but is not notarized yet. If macOS blocks the
first launch, open **System Settings > Privacy & Security** and choose
**Open Anyway** for Myan.

## Chrome And Arc

1. Install
   [Myan - Download Manager from the Chrome Web Store](https://chromewebstore.google.com/detail/myan-download-manager/dlclcdohlkfonkheoofpmfeinhjojdne).
2. Open **Myan - Download Manager.app** once if you have not already done so.

The extension can automatically transfer supported downloads to Myan. It also
adds **Download with Myan** to the link context menu.

## Safari

**Myan Browser Connector** will be available from the Mac App Store after
Apple completes the current review. The GitHub release does not distribute a
separate extension ZIP.

After installation:

1. Open **Myan Browser Connector** once.
2. Open **Safari > Settings > Extensions**.
3. Enable **Myan Download Extension** and allow access to websites.

Safari can automatically capture direct downloadable links. Downloads created
from `blob:` URLs, JavaScript, forms, or protected media may require the
**Download with Myan** context menu.

## Verify Downloads

Each release includes `SHA256SUMS.txt`.

```bash
shasum -a 256 -c SHA256SUMS.txt
```

## Beta Limitations

- The current build supports Apple Silicon only.
- App restart does not yet restore paused downloads.
- Browser extensions are distributed only through their official stores.
- Safari cannot intercept every browser-generated download.

This repository contains release documentation only. Application source code
is not published here.
