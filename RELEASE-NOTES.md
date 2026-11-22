**[Download for Windows (.exe)](https://github.com/Godchi872/GrabThis/releases/download/v0.1.58/GrabThis-0.1.58-Setup.exe)**

- Faster multi-connection file downloads and authenticated browser-session transfers (eliminated per-MB disk fsync stalls, batched progress checkpoints, incremental SHA-256, and single-row database updates).
- Expanded video quality support: 2K/4K and WebM/MKV/MOV video streams are now discovered and remuxed cleanly into MP4 (native MP4 streams remain preferred where available), and empty temporary media staging folders are removed automatically on completion.
- More resilient desktop UI refresh loop with automatic recovery on transient storage errors and lower polling overhead, plus updated `GrabThis/0.1` HTTP user-agent.
- Companion remains **0.1.29** (no Chromium extension reload is needed if updating from 0.1.57). Install over your existing version to preserve history, preferences and offline setup.
