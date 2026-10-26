# Changelog

## 0.1.53 - October 26, 2026

Windows update installers now use `%LOCALAPPDATA%\GrabThis\updates`. The existing download database and preferences stay in place, so changing the update-cache name does not reset history or interrupt the browser companion. Isolated diagnostics keep their own update folder.

Browser companion remains 0.1.26. This release contains only the Windows installer.

## 0.1.52 - October 26, 2026

Extension setup now includes an offline animated guide, shorter folder-selection instructions and connection/update reminders. Check for updates remains available in the sidebar. Completed downloads show only relevant actions, and opening a completed item closes its progress window. Registered Windows installations repair stale startup targets.

The verified first-party updater no longer adds the extra Internet-origin marker; cached installers lose only the exact marker written by earlier GrabThis updaters, after SHA-256 verification. Ordinary download handling and existing browser/Windows metadata are preserved. Older app versions can still display their existing Windows confirmation when installing this release.

Browser companion remains 0.1.26. Windows x64 only; no Linux package is published in this release.

## Firefox companion 0.1.26 - October 25, 2026

The signed companion is now available on [Mozilla Add-ons](https://addons.mozilla.org/en-US/firefox/addon/grabthis-download-companion/). Install directly with Add to Firefox; store extension updates are automatic when enabled in Firefox. Includes the floating-button hide control, improved video detection, browser-session file transfers and connection reporting. The desktop app remains **0.1.51**.

## 0.1.51 - HTTPS and video dependency security

Updates the video runtime to CPython 3.14.9, certifi 2026.10.19 and Brotli 1.2.1. Native downloads and update checks additionally reject all eight compromised eMudhra public keys while retaining normal TLS and hostname validation. Setup always replaces the video extractor and reuses unchanged FFmpeg files only after hash verification.

The optional curl-cffi impersonation backend is excluded until its separate vulnerable Brotli decoder is patched; sites that require it may be temporarily unavailable. Browser companion remains 0.1.26.

## 0.1.50 - filename safety and release checks

Removes misleading direction controls from new download filenames while preserving Arabic and other Unicode names. Confirmation and progress windows show the actual file extension; existing file paths are preserved. The website enforces a strict Content Security Policy and refuses unwanted framing. Releases now build from tracked source and pinned, verified tools with locked packages, regression/advisory gates, a component inventory and source-revision records. Publisher signing remains optional and unsigned preview status is unchanged. Companion remains 0.1.26.

## 0.1.49 - download security

Windows downloads now retain Internet-origin metadata, including browser-assisted files, media and update installers. Windows attachment policy and filesystems without named streams are respected. The bundled Node runtime is updated to 26.12.1 with pinned checksums. Privacy text explains browser-session file transfers, and update progress uses a clean separator. Companion remains 0.1.26.

## 0.1.48 - Drive archive redirects

Fixes the original-source check for Google Drive folder ZIPs that redirect to Google sign-in. These links now reach the browser-assisted transfer path instead of silently falling back during the native probe. Also fixes the garbled separator in the update dialog. Companion remains 0.1.26.

## 0.1.47 - browser-session downloads

Companion 0.1.26 adds browser-assisted transfers for eligible signed-in downloads, including Google Drive folder ZIP links. The browser reads the file using its existing session and GrabThis saves it with progress, pause/resume and integrity checks. Cookies stay in the browser. Keep the browser open during these transfers.

Unsupported resume or a changed source requires a restart without appending incorrect data. Rejected session responses safely return the original download to the browser. Reload the unpacked Chromium extension after installing this update.

## 0.1.46 - interactive update startup

Updates now pass the app language directly to Setup, preventing the language-selection dialog from delaying the installer readiness signal and application shutdown. The updater shows preparation and Windows-approval status, and restores the ready message when confirmation is cancelled. The modal updater closes before the main window; local handoff diagnostics record preparation, readiness and failures.

When installing this fix from 0.1.43-0.1.45, select the installer language promptly if asked. Companion remains 0.1.25.

## 0.1.45 - hide the floating button per video

Companion 0.1.25 adds a small close control on hover or keyboard focus (always available on touch devices). It hides the floating button for the selected video until the page is refreshed, without changing other videos or adding a permanent setting. Pending format lookups cannot restore a dismissed button.

After installing the update, reload the unpacked Chromium extension and confirm version 0.1.25.

## 0.1.44 - LinkedIn video capture

Companion 0.1.24 reads per-video source metadata on LinkedIn public players, including players with no direct src or a browser-local blob. It selects the highest declared bitrate from valid LinkedIn CDN sources and resets formats when the selected video changes. Downloads still require explicit confirmation.

After installing the update, reload the unpacked Chromium extension and confirm version 0.1.24. Firefox permanent distribution requires Mozilla signing.

## 0.1.43 — safe update installation

Install update asks for confirmation, pauses active transfers and saves their progress. GrabThis closes only after the elevated installer confirms readiness. Declining confirmation leaves work running; cancelling Windows approval, launch failure or cache revalidation failure keeps the app open and recovers previously running transfers. Manually paused jobs remain paused. Active MP3 conversions require restarting, with an explicit warning.

The installer cleans up reused media tools on uninstall and removes its directory only when empty. Versions 0.1.42 and earlier must be exited manually once when installing this fix.

## 0.1.42 — organized installation folder

GrabThis.exe remains the application entry point. Runtime libraries, configuration and the browser host are grouped in app; the uninstaller lives in app/uninstall. Tools, extensions, documentation and licenses have dedicated folders. Application libraries and the browser host use consistent GrabThis filenames.

Upgrading removes the previous flat runtime files, refreshes browser registrations and shortcuts, and reuses unchanged media tools. Existing extension paths and user data are preserved. The bundled runtime remains self-contained.

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
