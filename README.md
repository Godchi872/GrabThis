# GrabThis Download Manager

Your downloads. Under control.

[Website](https://grabthis.vercel.app/) · [Download](https://github.com/Godchi872/GrabThis/releases) · [Browser setup](docs/BROWSER-SETUP.md) · [Support on Ko-fi](https://ko-fi.com/grabthis)

![GrabThis desktop interface with example files](.github/assets/app-dark.webp)

GrabThis brings the important download tools together in a simple interface: automatic browser capture, pause and resume, video formats, and MP3 conversion.

## Features

- Capture eligible HTTP(S) downloads with a clear Start / Cancel / Download in browser confirmation.
- Pause and resume supported sources, choose automatic connections, and set a speed limit.
- Select available MP4 and MP3 options from a floating video button. YouTube prepares formats automatically; other supported sites inspect after a click.
- Convert local videos to MP3 without changing the original file.
- Organize videos, audio, files and programs, search history, and manage several downloads together.
- Light and dark appearance, English / Français / العربية, completion notifications and a notification-area icon.

## Download and install

Download **[GrabThis-0.1.36-Setup.exe](https://github.com/Godchi872/GrabThis/releases/download/v0.1.36/GrabThis-0.1.36-Setup.exe)** for Windows x64.

1. Open Setup.exe and choose the installation folder. It downloads and verifies the video tools (about 105 MB) and registers the local browser connection automatically.
2. Open **GrabThis** from the Desktop or Windows Start Menu shortcut. No terminal, .NET SDK or administrator account is required.
3. Follow the [browser setup guide](docs/BROWSER-SETUP.md). Both extension folders are installed beside the app; **Start Menu → GrabThis → Browser extensions** opens the Chrome/Edge folder.

The window X hides GrabThis in the notification area; use its tray menu’s Exit to quit. Uninstalling preserves your download history, preferences and downloaded files.

This is an unsigned preview build. Available video formats depend on the source; protected/private media and browser-only sessions may be unsupported. Resume and multiple connections require source support. This release contains the Windows x64 application. The older ZIP is retained as an advanced portable option; GitHub’s Source code archives contain documentation, not the app.

## Browser companion

Chrome and Edge currently use **Developer mode → Load unpacked**, with instructions in the package. The companion version in this release is **0.1.21**.

Firefox store submission is in progress. Until the signed listing is publicly available, the included unsigned Firefox package is a development preview; its temporary installation disappears when Firefox restarts. The setup guide identifies this limitation. No Android version is distributed.

## Feedback

Report a reproducible issue or suggest a feature in [Issues](https://github.com/Godchi872/GrabThis/issues). Include the app/companion versions and steps to reproduce. Avoid posting cookies, private URLs, access tokens or your download database.

This repository contains public release downloads, documentation and issue tracking. The desktop application's source is maintained separately. Third-party software retains its own licenses; included runtime notices are shipped with the application, and the video setup downloads upstream tools directly.

## Support

GrabThis is free to use. Optional support: [ko-fi.com/grabthis](https://ko-fi.com/grabthis).

[Privacy information](https://grabthis.vercel.app/privacy/)
