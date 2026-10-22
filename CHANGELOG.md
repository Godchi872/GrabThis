# Changelog

## 0.1.38 preview — in-app updates

Check for published updates automatically on startup and every six hours, with a dismissible banner. Settings includes Check for updates and the installed version. Download the Windows installer inside the app, with progress and cancellation; verified downloads expose an Install update button. The installer is never launched automatically.

Updates come from this project’s public GitHub releases, including published previews. Versions must be newer and the exact Windows installer asset must have a matching SHA-256 digest. Cached installers are checked again before launch. Interrupted or unverified temporary files are removed. The browser companion remains 0.1.22.

Versions before 0.1.38 require one manual Setup installation to enable future update checks. Unpacked extensions still require a browser Reload after upgrades that change the companion.

## 0.1.37 preview — companion 0.1.22

Keep the original Chromium browser GET download URL across redirects so supported sources can issue fresh temporary links after a pause. Stopped file downloads also offer **Update link**: paste a fresh URL for the same file, then resume. Existing parts and identity checks are preserved; changed files require a restart.

Completed progress windows now show Open file, Open folder, Show details and Close in one row. Removed the disabled Completed/Cancel actions.

After upgrading, reload unpacked browser extensions. Previously saved direct temporary links may need Update link. Firefox store submissions are managed separately.

## Windows installer â€” companion 0.1.21

Added a per-user Setup.exe with Desktop/Start Menu shortcuts, automatic native browser registration, verified video-tool setup, and both extension folders beside the app. No terminal commands are required. Reinstallation reuses prepared tools; uninstall preserves user data. Companion connection help now points to Setup for repair.

## 0.1.36 preview â€” companion 0.1.20

First public portable Windows preview. Includes automatic eligible file capture, supported pause/resume and connections, video format selection, local MP3 conversion, categories/search/bulk actions, notifications, tray controls, optional startup and English/French/Arabic light/dark UI.

The companion uses a translucent format menu, limits YouTube watch-page targeting to the main player, and constructs vector icons without HTML string parsing.

The portable launcher prepares verified official video tools on first run. Firefox store review is separate from this application release.
