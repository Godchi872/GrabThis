# Connect your browser

Install GrabThis using **Setup.exe**. It registers the local Chrome, Edge and Firefox connection automatically. Open GrabThis from the Desktop or Start Menu shortcut.

## Chrome / Edge

1. Open **Start Menu → GrabThis → Browser extensions**. Copy the folder address from File Explorer.
2. Open chrome://extensions in Chrome, or edge://extensions in Edge.
3. Enable Developer mode, choose Load unpacked and select that **extension** folder containing manifest.json. Both extension and extension-firefox are beside Idman.exe in the installation folder.
4. Keep GrabThis Download Companion enabled and allow site access for the websites you use. Its popup should report the desktop app as connected.
5. After installing an updated GrabThis version, click the circular Reload arrow in its extension card and check its version. The page-wide Update button does not fetch new files for an unpacked extension.

Private windows require a separate Allow in Incognito / InPrivate permission in the extension’s Details.

## Firefox

Setup registers the Firefox native connection automatically. The signed Firefox store listing is not yet confirmed as available. The unsigned preview can be tested through about:debugging#/runtime/this-firefox → Load Temporary Add-on → extension-firefox/manifest.json in the installed application folder. Firefox removes temporary add-ons when it restarts. Do not disable signing checks. The public store link will replace these preview instructions once available.

## Troubleshooting

If disconnected, open GrabThis, rerun **Setup.exe** to repair the connection and reload the extension. Refresh an already-open video page if an old message remains. Another download manager may intercept a request first.

Ordinary GET file downloads can be captured. POST, blob, protected/login-only and browser-only downloads may remain in the browser or be unavailable. Very fast Firefox files may finish before capture.

## Français / العربية

Open **Browser setup guide** from GrabThis’s Start Menu folder for the included English, French and Arabic instructions. Localized website guides: https://grabthis.vercel.app/fr/#setup and https://grabthis.vercel.app/ar/#setup.
