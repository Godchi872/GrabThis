GrabThis 0.1.37 — resume and progress-window fixes

Download **GrabThis-0.1.37-Setup.exe**, open it and install. Setup includes companion **0.1.22** and registers the desktop browser connection. Launch GrabThis from its Desktop or Start Menu shortcut.

- Chromium browser capture keeps the original GET URL across redirects, allowing fresh temporary download links from supported sources after a pause.
- **Update link** on stopped file downloads lets you paste a fresh URL for the same file. Downloaded parts and file-identity checks are preserved. A different file requires restarting; sources must support resuming.
- Completed progress windows show Open file, Open folder, Show details and Close together, without disabled Completed/Cancel actions.

**After upgrading:** reload the unpacked extension from your browser's Extensions page. Downloads saved with direct temporary URLs, including Firefox captures where only the resolved URL is available, may need Update link. The Firefox unsigned package is a development preview; Mozilla signing and store publication are separate.

Validation: local renewable-link expiry/recovery, preserved partial data, changed-file rejection, downloader regression checks, real WPF controls in English/French/Arabic and both themes, Chrome capture/ownership checks, Firefox capture/fallback/redirect handoff and isolated installer checks. Windows x64 preview, unsigned installer. Setup downloads about 105 MB of verified video tools on first installation. SHA256SUMS.txt accompanies this release.
