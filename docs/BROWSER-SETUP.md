# Add GrabThis to your browser

Install the desktop app with **[GrabThis Setup.exe](https://github.com/Godchi872/GrabThis/releases/download/v0.1.53/GrabThis-0.1.53-Setup.exe)** first. Setup registers the local browser connection automatically.

On first launch, **Extension setup** opens automatically. Chrome, Edge and Brave share a five-step illustrated guide; Firefox has its own button opening the [Firefox Add-ons page](https://addons.mozilla.org/en-US/firefox/addon/grabthis-download-companion/). **Finish** closes the guide even while connection verification is pending. The reminder stays visible until a verified connection is completed; reopen the guide from the sidebar at any time.

Setup installs in **Program Files** and requests administrator approval for installation and updates. The app itself runs with normal user permissions. On the first launch after upgrading a previous per-user installation, GrabThis removes the old program while preserving user data and existing unpacked-extension folders.

Open **Start Menu → GrabThis → Browser extensions**. Copy the folder address from File Explorer; you will select this folder in step 3.

## Chromium browsers

Chrome, Edge, Brave, Opera / Opera GX and other compatible Chromium browsers use the same **extension** folder. Watch the complete illustrated guide below, or open the individual picture steps.

### Watch the complete setup

From the browser’s three-dot menu through Developer mode, Load unpacked, choosing the extension folder and checking that GrabThis is enabled. This is an illustrated Chrome example; labels can vary in Edge, Brave and Opera. No personal folder names are used.

![Complete illustrated browser setup for GrabThis](../.github/assets/guides/browser-setup.gif)

<details>
<summary>Step-by-step images</summary>

### Open Extensions without typing an address

In Chrome, click the **three dots → Extensions → Manage extensions**. Other Chromium browsers may offer Extensions directly in their menu or under More tools.

![Illustrated menu: three dots, Extensions and Manage extensions](../.github/assets/guides/00-browser-menu.svg)

This numbered menu image is an illustration. The following Developer mode and Load unpacked images are actual browser screenshots.

**Or copy the address for your browser:**

| Browser | Extensions page |
| --- | --- |
| <img src="../.github/assets/browsers/chrome.svg" width="20" height="20" alt=""> Chrome | `chrome://extensions` |
| <img src="../.github/assets/browsers/edge.svg" width="20" height="20" alt=""> Microsoft Edge | `edge://extensions` |
| <img src="../.github/assets/browsers/brave.svg" width="20" height="20" alt=""> Brave | `brave://extensions` |
| <img src="../.github/assets/browsers/opera.svg" width="20" height="20" alt=""> Opera / Opera GX | `opera://extensions` |

Screenshots use Chrome. Labels and control positions can vary slightly between browsers.

### 1. Turn on Developer mode

Open the extensions page for your browser from the table above. Turn on **Developer mode**, outlined in orange in the screenshot.

![Step 1: Developer mode highlighted with rectangle number 1](../.github/assets/guides/01-developer-mode.png)

### 2. Click Load unpacked

The button appears after Developer mode is enabled. Click the highlighted **Load unpacked** button.

![Step 2: Load unpacked highlighted with rectangle number 2](../.github/assets/guides/02-load-unpacked.png)

### 3. Choose the extension folder

In the folder picker, select **extension** inside the installed GrabThis folder. You can paste the address copied from File Explorer. Select the folder itself; it contains **manifest.json**. Choose **extension**, rather than **extension-firefox** or the installer file.

Open **This PC → Local Disk (C:) → Program Files → GrabThis**. Select **extension**, then click **Select Folder**. The short animation starts at This PC and shows the default installation path. Unrelated folders are blurred.

![Illustrated folder selection: This PC, Local Disk C, Program Files, GrabThis, extension, Select Folder](../.github/assets/guides/extension-folder.gif)

### 4. Check that GrabThis is enabled

The **GrabThis Download Companion** card should appear with its switch on. Open the desktop app. The companion’s toolbar popup should show the desktop app as connected.

![Step 4: enabled GrabThis switch highlighted with rectangle number 4](../.github/assets/guides/04-extension-ready.png)

</details>

Allow site access for the websites you use. Private windows require a separate **Incognito / InPrivate / private-window** permission, where available, in the extension’s Details.

### Updating the extension

Install the updated GrabThis version, then click the circular **Reload** arrow inside its extension card and check the version. The page-wide Update button does not download new files for an unpacked extension.

## Firefox

Companion **0.1.26** is published and signed on Mozilla Add-ons. No Developer mode or temporary installation is needed.

1. Install and open the GrabThis desktop app. Setup registers the Firefox connection automatically.
2. Open **[GrabThis Download Companion on Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/grabthis-download-companion/)**, or use the app's **Firefox Store** button.
3. Choose **Add to Firefox** and approve the requested permissions.
4. Open the extension's toolbar popup to check the desktop connection, then refresh video pages that were already open.

Firefox installs future store extension updates automatically when automatic add-on updates are enabled. To check manually, open **Add-ons and themes → Extensions**, then choose **Check for Updates** from the gear menu. Desktop app updates are handled separately inside GrabThis.

The included **extension-firefox** folder is for development testing; use the signed store version for normal installation.

## Hide the floating button

Hover over GrabThis on a video and click **×**. The button stays hidden for that video until you refresh the page; other videos keep their buttons. Keyboard users can Tab to the close button and press Enter. No permanent site setting is changed.

## Troubleshooting

**Desktop app disconnected:** open GrabThis, rerun Setup.exe to repair the connection and reload the extension. Refresh an already-open video page if an old message remains.

**A file stays in the browser:** another download manager may intercept it first. POST, blob, protected/login-only and browser-only sessions may remain in the browser or be unavailable. Very fast Firefox files may finish before capture.

**A video has different qualities:** formats depend on the source. YouTube prepares the main video automatically; other sites inspect the selected video after you click the button.

## Français / العربية

The same illustrated guide is available on the localized website:

- [Français](https://grabthis.vercel.app/fr/#chrome-setup)
- [العربية](https://grabthis.vercel.app/ar/#chrome-setup)

Open the Chromium browser setup section to watch the complete animation, or expand the individual picture steps. The included **Browser setup guide** in GrabThis’s Start Menu folder also contains English, French and Arabic instructions.

Browser references: [Brave extension compatibility](https://support.brave.com/hc/en-us/articles/360017909112-How-can-I-add-extensions-to-Brave) · [Opera Developer mode and unpacked extensions](https://help.opera.com/en/extensions/testing/).
