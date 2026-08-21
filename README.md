# 3D Ridgeline Landscape Explorer

An interactive, GPU-accelerated 3D topographic terrain explorer, finite element adaptive mesh visualizer, and Joy Division style ridgeline generator built with **Three.js** and **Delaunator**.

🌐 **Live Demo**: [https://jbcohn.github.io/Ridgeline-3D-Explorer/](https://jbcohn.github.io/Ridgeline-3D-Explorer/)

---

## ✨ Features

- **🏔️ 12 Real-World Topographic Regions**: Mt. Shasta, Mt. Whitney, Mt. Diablo, Mt. Tamalpais, Vaca Mountains, Lake Tahoe, Yosemite Valley, San Francisco Bay Area, and full California DEM relief.
- **🎨 3 Unique 3D Render Modes**:
  - **Gradual Adaptive Mesh**: Quality Delaunay TIN with spatial Poisson-disk sampling, Chew's second algorithm circumcenter refinement, and Centroidal Lloyd relaxation (dense geometry on mountain ridges and peaks).
  - **Uniform Wireframe Grid**: Classic FEA quad-tessellated finite element wireframe with jitter controls.
  - **Stacked Ridgelines**: Joy Division *Unknown Pleasures* style topographic elevation contour slices.
- **☀️ True HSL Lightness Shading**:
  - Slope-aware directional relief shading that modulates **only perceptual Lightness ($L$)** in HSL color space.
  - Preserves 100% color integrity (no muddy brown/olive shifts or specular whiteout).
  - Options for *Pure Vibrant Heatmap*, *Smooth Topography*, and *Faceted FEA 3D*.
- **✈️ Dual Navigation Modes**:
  - **Flight Mode**: Smooth WASD + Arrow keys / On-Screen Steering controls to fly through the 3D valleys and mountain canyons.
  - **Classic Orbit Mode**: Turntable rotation, smooth two-finger trackpad drag pan and zoom.
- **📱 Responsive Mobile UI**:
  - Collapsible desktop sidebar with glowing drag handle resizer.
  - Mobile bottom sheet with touch swipe gestures.
  - Floating on-canvas quick action buttons.
- **📸 Ultra High-Res PNG Export**:
  - Snapshot rendering up to **5000 × 5000 (5K Master Print)**.
  - Transparent print-ready background export with automatic occluding surface depth clipping.

---

## 🚀 Controls

| Action | Flight Mode | Orbit Mode |
|---|---|---|
| **Fly Forward / Backward** | `W` / `S` or `↑` / `↓` | — |
| **Strafe Left / Right** | `A` / `D` | — |
| **Climb / Descend** | `E` / `Q` or On-Screen Climb/Descend | — |
| **Turn View Direction** | `←` / `→` or Drag canvas | Drag canvas to Orbit |
| **Pan Camera** | Shift + Drag / Wheel | Shift + Drag / Wheel or PAN Mode |
| **Zoom In / Out** | Mouse Wheel / Trackpad Pinch | Mouse Wheel / Trackpad Pinch |
| **Toggle Menu** | ☰ Floating Button or Drag Handle | ☰ Floating Button or Drag Handle |

---

## 🛠️ Built With

- [Three.js](https://threejs.org/) — 3D Scene Graph & WebGL Rendering
- [Delaunator](https://github.com/mapbox/delaunator) — Fast 2D Delaunay Triangulation
- [Google Fonts (Outfit)](https://fonts.google.com/specimen/Outfit) — Modern UI Typography
- USGS 3D Elevation Program (3DEP) DEM Topography Data
