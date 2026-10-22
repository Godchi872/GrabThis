# Changelog

## 0.1.41 — installation and extension setup

Setup now defaults to Program Files, with shared shortcuts and browser registrations. Installation and updates request administrator approval; the app runs with normal permissions. On first launch, a previous per-user installation is migrated without changing download history or preferences. Existing unpacked-extension folders remain available to the browser.

Extension setup groups Chrome, Edge and Brave into one illustrated guide and provides a Firefox Store button. Finish remains usable while connection verification is pending. The installer offers a single launch checkbox; the guide opens inside the app.

## 0.1.40 — Windows notification branding

Windows completion notifications now consistently display GrabThis. Added an explicit Windows application identity and matching Start Menu/Desktop shortcuts. Browser native-host launching and portable entry points use the new executable.

Setup removes obsolete desktop binaries and preserves the existing download database, preferences and native messaging host identifiers. An existing startup command for the old executable in the same installation is migrated to the new path.

## 0.1.39 preview — first-run browser setup

A first-run wizard explains why the companion is needed and walks users through browser selection, the Extensions page, Developer mode, folder selection and connection verification. Offline images highlight the relevant controls and can be enlarged. Firefox has a separate temporary add-on path; its store button remains unavailable until a signed listing is confirmed and configured.

Set up later persists the dismissal, while a sidebar shortcut and reminder keep the guide accessible. Finish requires a recent native handshake from the selected browser with site access enabled. Companion 0.1.23 records only browser family, extension version, permission state and timestamp locally for this verification. The installer now explicitly registers Brave and Chromium too, and its final launch checkbox points users to browser setup.

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
