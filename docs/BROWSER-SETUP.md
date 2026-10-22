# Connect your browser

Start GrabThis once with START-GRABTHIS.cmd before connecting a browser. Keep the extracted application folder in a permanent location.

## Chrome / Edge

1. Run Connect-Browser.cmd in the application folder. It registers the local connection and copies the extension-folder path.
2. Open chrome://extensions in Chrome, or edge://extensions in Edge.
3. Enable Developer mode, choose Load unpacked and select the included **extension** folder containing manifest.json. Select the folder, not the ZIP or extension-firefox.
4. Keep GrabThis Download Companion enabled. Allow site access for the websites you use. Its popup should report the desktop app as connected.
5. To update an unpacked extension, replace its files in the same folder and click the circular Reload arrow inside the GrabThis card. The page-wide Update button does not fetch the new files.

Private windows require a separate Allow in Incognito / InPrivate permission in the extension's Details.

## Firefox

Run Connect-Firefox.cmd in the application folder to register the native connection for your Windows user account.

The signed Firefox store listing is not yet confirmed as available. The unsigned preview included here can be tested through about:debugging#/runtime/this-firefox → Load Temporary Add-on → extension-firefox/manifest.json. Firefox removes temporary add-ons when it restarts. Do not disable signing checks. The public store link will replace these preview instructions once available.

## Troubleshooting

If the desktop app is disconnected, open GrabThis, rerun the connector from the folder's current location and reload the extension. Refresh an already-open video page if an old message remains. Another download manager may intercept a request first.

Ordinary GET file downloads can be captured. POST, blob, protected/login-only and browser-only downloads may remain in the browser or be unavailable. Very fast Firefox files may finish before capture.

## Français / العربية

The portable package's **BROWSER-SETUP.txt** contains the complete English, French and Arabic instructions. The localized website guide is at https://grabthis.vercel.app/fr/#setup and https://grabthis.vercel.app/ar/#setup.
