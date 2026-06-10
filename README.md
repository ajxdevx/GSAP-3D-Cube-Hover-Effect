# GSAP 3D Cube Hover Effect

An interactive mosaic preview built with **GSAP** and **CSS 3D transforms**. Each tile is a mini cube that breathes in 3D space. Hover over a project name to flip the mosaic and reveal a new image with a staggered animation from the center outward.

**Author:** AJ

## Preview

Hover the project links in the bottom-right corner to switch images. The mosaic is made of 12×9 tiles (108 cubes), each with six faces. On hover, tiles rotate on the Y-axis with a center-out stagger while a subtle idle animation keeps the grid alive.

## Features

- 3D cube tiles with front, rear, side, top, and bottom faces
- GSAP staggered flip animation on project hover
- Continuous breathing motion on each tile
- Smooth queue handling when hovering quickly between projects
- Built with Vite for fast local development

## Tech Stack

- [GSAP](https://gsap.com/) — animations
- [Vite](https://vitejs.dev/) — dev server and bundler
- HTML, CSS, JavaScript

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)

### Installation

```bash
git clone https://github.com/ajxdevx/GSAP-3D-Cube-Hover-Effect.git
cd GSAP-3D-Cube-Hover-Effect
npm install
```

### Add Your Images

Place your images in the project root (or `public/` folder if you add one):

| File         | Purpose                          |
| ------------ | -------------------------------- |
| `default.jpg` | Default / idle preview image    |
| `img1.jpg`   | Project 1 (NX-09)                |
| `img2.jpg`   | Project 2 (1997 Hallway Tape)    |
| `img3.jpg`   | Project 3 (Deep Space)           |
| `img4.jpg`   | Project 4 (Sleep Phase Anomaly)  |
| `img5.jpg`   | Project 5 (Still-life.mov)       |
| `img6.jpg`   | Project 6 (Monoform™)            |

Recommended size: **720×540 px** (12 × 60 by 9 × 60).

### Run Locally

```bash
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

## Project Structure

```
├── index.html      # Page markup and project list
├── script.js       # Tile generation, GSAP animations, hover logic
├── styles.css      # 3D transforms, grid layout, typography
├── package.json
└── README.md
```

## Customization

- **Grid size:** Edit `TILES_X`, `TILES_Y`, and `TILE_SIZE` in `script.js`, and update the CSS grid in `styles.css`.
- **Project names:** Change the links in `index.html` and match `data-index` values to `PROJECT_IMAGES` in `script.js`.
- **Animation timing:** Adjust `duration`, `stagger.each`, and breathe ranges in `script.js`.

## License

ISC
