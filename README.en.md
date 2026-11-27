# BenJi · Offline ID Photo Tool

A single-file, browser-based ID photo maker that runs **completely offline**. AI background removal, standard-size cropping, background replacement, and print-sheet layout are all bundled into one HTML file. No installation, no internet connection, and your photos never leave your computer.

Current version: **v5.22**

## Download

- **Gitee Releases (primary, recommended in China)**: https://gitee.com/humbleperson/benji-idphoto/releases/latest
- GitHub Releases (mirror): https://github.com/ttisgood2025/benji-idphoto/releases/latest

Each release ships a single attachment, `idphoto.html`. Open it with a recent version of Chrome, Edge, or Firefox. You may rename it to any filename you like; renaming does not affect functionality.

## Quick start

1. **Upload a photo** — click the upload button on the left, or drag an image onto the canvas.
2. **Frame the subject** — drag to reposition and scroll (or use the slider) to zoom, keeping the person centered inside the blue guide. Everything outside the blue guide is cropped out on export; the live preview shows the final result.
3. **Pick a size and background** —
   - Choose a region (Chinese ID / US ID / International & Visa) and the exact spec you need (1-inch, 2-inch, passport, visa, etc.).
   - Pick white, blue, red, light blue, pink, grey, or set a custom background color.
   - Enable **Replace background** to activate AI cutout. Use the edge slider if stray pixels remain around hair.
4. **Export** —
   - **Single photo**: exported at the selected spec, with 300 DPI (standard) or 600 DPI (high resolution).
   - **Print sheet**: arrange multiple copies onto 5-inch, 6-inch, or A4 paper for a photo lab.

## Features

- **Offline-ready** — the AI model is embedded; background removal works without a network connection.
- **Privacy-first** — all processing happens locally in your browser. Photos are never uploaded.
- **Standard sizes** — covers common Chinese, US, and international visa photo specs.
- **One-click export** — single photo or print-sheet layout, at 300 or 600 DPI.
- **No installation** — one HTML file, double-click to open. No registry entries, no activation.

## Updating

Click **Check for updates** at the top right of the tool:

1. If it says "up to date", nothing to do. If a new version is found, confirm the prompt.
2. The browser downloads the new HTML automatically (no password, no archive). If nothing happens, the download page opens in a new tab — click there to download.
3. Overwrite your old file with the new one and reopen it in the same browser. Keep the filename and location unchanged.

Checking for updates requires internet access. Day-to-day cropping and exporting do not.

## FAQ

| Symptom | Fix |
|---|---|
| Blank page or broken layout | Use a recent Chrome, Edge, or Firefox |
| AI background removal fails | Enable WebGL in your browser; retry, or leave the background unchanged |
| Export download does nothing | Right-click the preview and choose "Save image as", or use "Copy to clipboard" |
| Settings reset on reopen | Check whether you switched browsers, used private mode, or moved the file |
| Exported JPG is small | Normal — JPEG compression is efficient and 300 DPI meets print standards. Choose 600 DPI for more detail |

## License

© 2026 Wenxin Zhou. Free for personal use and sharing, provided attribution is retained. **Commercial resale is prohibited**, with or without attribution. See [LICENSE](LICENSE) for the full terms.

This software includes MediaPipe Tasks Vision by Google LLC, distributed under the Apache License 2.0.

## About this repository

This repository distributes the built HTML file and release notes only. It does not contain source code. The tool is a standalone front-end application with no build step or dependencies to install.
