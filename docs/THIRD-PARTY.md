# Third-party video tools

GrabThis runs its video tools as separate programs. Their licenses and copyright
notices remain their own; the installed `licenses` folder includes the bundled
FFmpeg GPL text, Node.js notices, .NET notices and media-runtime notices.

## FFmpeg included in Windows 0.1.54

- Upstream build: `ffmpeg-N-127911-gadfe258a6a-win64-gpl-shared`.
- License: [GNU GPL version 3](https://www.gnu.org/licenses/gpl-3.0.html).
- [Exact FFmpeg source tree](https://github.com/FFmpeg/FFmpeg/tree/adfe258a6a8ff1423f413c94e2606fc95cc003dd).
- [Download that FFmpeg source](https://github.com/FFmpeg/FFmpeg/archive/adfe258a6a8ff1423f413c94e2606fc95cc003dd.tar.gz).
- [Build scripts, dependency recipes and source locations](https://github.com/yt-dlp/FFmpeg-Builds/tree/596b25ea84a6bf6a2fe074a234c04aba794657ce).
- [Exact upstream binary release and checksums](https://github.com/yt-dlp/FFmpeg-Builds/releases/tag/autobuild-2026-10-21-18-38).
- [Recorded upstream build run and download cache](https://github.com/yt-dlp/FFmpeg-Builds/actions/runs/39650984019).

FFmpeg and its shared libraries are copied unchanged from that verified upstream
Windows archive. Other bundled tools retain the licenses identified in the
release SBOM and installed notices. These upstream source links concern those
third-party components; GitHub's automatic Source code ZIP for the GrabThis
release contains this documentation repository.

## Other components

- [yt-dlp source and license](https://github.com/yt-dlp/yt-dlp).
- [Node.js source and license](https://github.com/nodejs/node/tree/v26.12.1).
- [.NET runtime source and license](https://github.com/dotnet/runtime).

Each release includes a component inventory and exact input hashes in its SBOM
and build-info assets.
