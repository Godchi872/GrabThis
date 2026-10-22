GrabThis 0.1.38 — direct in-app updates

GrabThis checks its public GitHub releases at startup and every six hours. A dismissible banner announces newer published versions. Settings shows the installed version and includes Check for updates.

Choose Update, then Download update to fetch Setup.exe inside the app with progress and cancellation. After the exact file size and SHA-256 digest are verified, choose Install update to launch Setup. Cached installers are rechecked before launch. Download failures and offline checks leave ordinary transfers running; the installer is never launched automatically.

**First installation of this feature:** versions before 0.1.38 cannot discover updates themselves. Download GrabThis-0.1.38-Setup.exe once and install it over your existing version. Downloads and preferences are preserved. Browser companion remains 0.1.22; this release does not update extension files automatically inside the browser.

Checks passed: numeric version comparison and preview selection; equal/older/draft/external or unverified asset rejection; downloaded/cached installer hash verification; tampering, truncated response, cancellation and offline handling; real WPF manual check, update banner, direct-download and ready-to-install states in English/French/Arabic and both themes. The actual public GitHub feed was checked separately. Installer execution itself is user-controlled and was not triggered by update diagnostics.

Windows x64 preview, unsigned installer. Setup prepares verified media tools as before. SHA256SUMS.txt accompanies this release.
