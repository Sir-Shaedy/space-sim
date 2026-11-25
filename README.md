# Eclipse NG — 3D Orbit & Real-Time Astronomical Solver

An interactive, single-file WebGL solar-system simulator that runs entirely in the browser.

![Single file](https://img.shields.io/badge/build-none%20required-brightgreen?style=flat-square)
![WebGL](https://img.shields.io/badge/WebGL-2.0-blue?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=flat-square)

## Live Demo

Deployed via GitHub Pages: **https://sir-shaedy.github.io/space-sim/**

## Features

- Real-time 3D orbital simulation rendered with raw WebGL (no framework, no build step)
- Astronomical solver for planetary positions, eclipse detection, and event prediction
- Swappable Earth/planet surface textures streamed from public tile services
  (NASA GIBS, Esri World Imagery, ArcGIS Ocean & Shaded Relief)
- Floating glass UI with segmented navigation, optimized for desktop and touch devices

## Run Locally

There is nothing to install. Just open the file:

```bash
# simply double-click index.html, or serve it:
python3 -m http.server 8000
# then visit http://localhost:8000
```

A local HTTP server is recommended so that CORS-restricted texture tiles load correctly.

## Structure

```
index.html   # the entire application (markup, styles, and WebGL/astronomy engine)
```

## Notes

Map tiles are fetched from third-party public endpoints at runtime and require a
network connection. The astronomy/orbital math and rendering are fully local.

## License

MIT
