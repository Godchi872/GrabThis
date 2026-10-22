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

## Download and run

The current preview release contains a **Windows x64 portable package**. Choose the file ending in `windows-x64.zip` in [Releases](https://github.com/Godchi872/GrabThis/releases). GitHub's automatically generated Source code archives contain this documentation, not the desktop app.

1. Extract the whole ZIP into a folder you want to keep.
2. Open **START-GRABTHIS.cmd**. On first launch it downloads the pinned, SHA-256-verified video tools from their official GitHub releases (about 105 MB). Subsequent launches reuse them. No .NET SDK or administrator account is needed.
3. Follow the [browser setup guide](docs/BROWSER-SETUP.md) to connect Chrome, Edge or Firefox.

Keep the application folder together. If you move it, rerun the relevant connector and load the unpacked extension from its new folder. The window X hides GrabThis in the notification area; use the tray menu's Exit to quit.

This is an unsigned preview build. Available video formats depend on the source; protected/private media and browser-only sessions may be unsupported. Resume and multiple connections require source support. This Windows archive contains no Linux executable.

## Browser companion

Chrome and Edge currently use **Developer mode → Load unpacked**, with instructions in the package. The companion version in this release is **0.1.20**.

Firefox store submission is in progress. Until the signed listing is publicly available, the included unsigned Firefox package is a development preview; its temporary installation disappears when Firefox restarts. The setup guide identifies this limitation. No Android version is distributed.

## Feedback

Report a reproducible issue or suggest a feature in [Issues](https://github.com/Godchi872/GrabThis/issues). Include the app/companion versions and steps to reproduce. Avoid posting cookies, private URLs, access tokens or your download database.

This repository contains public release downloads, documentation and issue tracking. The desktop application's source is maintained separately. Third-party software retains its own licenses; included runtime notices are shipped in the Windows archive, and the video setup downloads upstream tools directly.

## Support

GrabThis is free to use. Optional support: [ko-fi.com/grabthis](https://ko-fi.com/grabthis).

[Privacy information](https://grabthis.vercel.app/privacy/)
