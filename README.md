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

1. Download `Myan-Chrome-Arc-Extension-*.zip`.
2. Extract the ZIP to a permanent folder. Do not delete that folder while the
   extension is installed.
3. Open `chrome://extensions` in Chrome or `arc://extensions` in Arc.
4. Enable **Developer mode**.
5. Click **Load unpacked** and select the extracted extension folder.
6. Open **Myan - Download Manager.app** once if you have not already done so.

The extension can automatically transfer supported downloads to Myan. It also
adds **Download with Myan** to the link context menu.

## Safari

1. Download `Myan-Safari-Extension-*.zip`.
2. Extract the ZIP.
3. Move **Myan Safari Extension.app** to `/Applications`.
4. Open the Safari extension app once.
5. In Safari, open **Settings > Extensions**.
6. Enable **Myan Safari Extension** and allow access to websites.

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
- Chrome and Arc require Developer mode until the extension is published in
  the Chrome Web Store.
- Safari cannot intercept every browser-generated download.

This repository contains release documentation only. Application source code
is not published here.
