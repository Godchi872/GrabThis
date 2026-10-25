# Install and update GrabThis

## Install on Windows

1. Download **[GrabThis-0.1.51-Setup.exe](https://github.com/Godchi872/GrabThis/releases/download/v0.1.51/GrabThis-0.1.51-Setup.exe)** and open it.
2. Approve the Windows administrator prompt. Setup installs in **Program Files** and prepares the video tools and browser connection. An internet connection is needed for about 105 MB of verified tools.
3. Open **GrabThis** from the Desktop or Start Menu shortcut.
4. Follow **Extension setup** on first launch. Chrome, Edge and Brave share an illustrated guide; Firefox has its own Add-ons button. Opera and other compatible Chromium browsers can follow the [browser guide](BROWSER-SETUP.md#chromium-browsers).

The app runs with normal user permissions. Installation and updates need administrator approval. No terminal or .NET SDK is required. The installer is an unsigned preview. [Release notes and checksums](https://github.com/Godchi872/GrabThis/releases/tag/v0.1.51) are available with the download.

Choose **Setup.exe** in GitHub’s release assets. The automatically generated Source code archives are not the Windows installer.

## Connect the browser

The installer registers the local desktop connection. Adding the extension to each browser requires your approval. You can reopen **Extension setup** from the sidebar at any time.

- **Chromium browsers:** open **Start Menu → GrabThis → Browser extensions**, then follow the [highlighted screenshots](BROWSER-SETUP.md#chromium-browsers) to load the **extension** folder.
- **Firefox:** use the app’s Firefox Store button or the [Firefox Add-ons listing](https://addons.mozilla.org/en-US/firefox/addon/grabthis-download-companion/). Signed version **0.1.26** is available; choose **Add to Firefox**. No Developer mode is required.

The included **extension-firefox** folder is a development package for temporary testing; permanent installation uses Mozilla’s signed distribution. Companion version: **0.1.26**.

## Updates inside the app

From version **0.1.38**, GrabThis checks for updates at startup and every six hours. You can also open **Settings → Check for updates**.

1. Download the update inside GrabThis. The app shows progress and verifies the installer’s size and SHA-256.
2. Choose **Install update**, then confirm **Close and install**.
3. Approve Windows’ prompt. From **0.1.46**, updates automatically use the app language, so no separate language-selection dialog blocks shutdown. From **0.1.43**, GrabThis saves download progress and closes automatically once the installer is ready. Continue through Setup and reopen the app; resume saved downloads when ready.

If you cancel Windows approval or the installer cannot start, GrabThis stays open and resumes previously running downloads. A running local conversion is stopped for installation and must be restarted.

**Updating from 0.1.42 or earlier:** exit the old app from its tray menu once before installing this fix. Future updates handle closing automatically.

Firefox store extensions update automatically when automatic add-on updates are enabled. For manual checks, see the [Firefox guide](BROWSER-SETUP.md#firefox).

For an unpacked Chromium extension update, install the updated app, then click **Reload** on its browser extension card. [Extension update details](BROWSER-SETUP.md#updating-the-extension).

## Downloads that need your browser session

From app **0.1.47** and companion **0.1.26**, eligible signed-in downloads can transfer through the browser session into GrabThis. Keep the same browser open with the extension enabled. Cookies stay inside the browser. Pause and resume depend on the server; an expired or changed source may require starting again from the website. Private-window session downloads stay in the browser.

Install the new app and reload the Chromium extension before testing this feature. Firefox users can install the signed **0.1.26** extension from the [Mozilla Add-ons listing](https://addons.mozilla.org/en-US/firefox/addon/grabthis-download-companion/).

## Existing installations and uninstalling

Setup upgrades the machine installation. When migrating a previous per-user installation, GrabThis removes the old program on its first normal launch while preserving user data and existing unpacked-extension folders.

Uninstalling preserves your download history, preferences and downloaded files.

[Back to GrabThis](../README.md) · [Troubleshooting](BROWSER-SETUP.md#troubleshooting)
