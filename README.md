  _______________________________.____    .____       _____ __________    ___ ___    _____    _______  ________    _________
 /   _____/\__    ___/\_   _____/|    |   |    |     /  _  \\______   \  /   |   \  /  _  \   \      \ \______ \  /   _____/
 \_____  \   |    |    |    __)_ |    |   |    |    /  /_\  \|       _/ /    ~    \/  /_\  \  /   |   \ |    |  \ \_____  \ 
 /        \  |    |    |        \|    |___|    |___/    |    \    |   \ \    Y    /    |    \/    |    \|    `   \/        \
/_______  /  |____|   /_______  /|_______ \_______ \____|__  /____|_  /  \___|_  /\____|__  /\____|__  /_______  /_______  /
        \/                    \/         \/       \/       \/       \/         \/         \/         \/        \/        \/ 

.   *    .       *    .        *    .    *
    *       .        *      .       *         .
       ✋ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ > * . ° ✨
    .       *    .       *    .        *    .
        *      .     *      .      *      .     *
    .
# ✦ STELLAR — Particle Field Engine

<div align="center">

**Real-time hand-tracked particle physics in the browser.**  
150,000 particles. 8 gestures. 10 formations. Zero dependencies beyond a webcam.

[Live Demo](#) · [Report Bug](https://github.com/ayuuXploits/stellar/issues) · [Request Feature](https://github.com/ayuuXploits/stellar/issues)

</div>

---

## 🌌 Overview

STELLAR is a GPU-accelerated particle field engine that uses your webcam and hand pose estimation to interact with 150,000 real-time particles rendered via Three.js. Point, pinch, slash, or freeze the field — each gesture triggers a distinct physics behaviour.

No backend. No build step. Open the HTML file and go.

---

## ✨ Features

- **150,000 live particles** rendered with additive blending via WebGL
- **8 hand gestures** mapped to unique particle physics effects
- **10 cosmic formations** — Galaxy, Nebula, Black Hole, Saturn, DNA, Crystal, Torus, Supernova, Starship, Spacecraft
- **MediaPipe Hands** AI model for real-time pose detection
- **Mouse fallback** — fully interactive without a webcam
- **Slash detection** — draw a fast swipe to trigger a shockwave
- **Hold-to-freeze** — hold a fist to suspend the entire field
- **Live skeleton overlay** in the camera preview with per-finger colours
- **Grain + vignette film overlays** for cinematic aesthetic

---

## 🤌 Gesture Reference

| Gesture | Effect |
|---|---|
| ✊ **Fist** | Implode — collapse particles toward hand |
| 🤏 **Pinch** | Attract — draw particles inward |
| ☝ **1 Finger** | Laser — horizontal pierce beam |
| ✌ **2 Fingers** | Scissor — split the field left/right |
| 🖐 **Open Hand** | Repel — burst particles outward |
| 👌 **OK Sign** | Vortex — orbital spin around hand |
| ⏸ **Hold Fist** | Freeze — suspend the entire field |
| ⚡ **Slash** | Shockwave — fast swipe cuts through the field |

---

## 🚀 Getting Started

### Prerequisites

- A modern browser with WebGL support (Chrome / Edge recommended)
- A webcam (optional — mouse works as fallback)

### Run Locally

```bash
git clone https://github.com/ayuuXploits/stellar.git
cd stellar
# Open index.html directly in your browser — no build step required
open index.html
```

Or serve it locally for camera access:

```bash
npx serve .
# then visit http://localhost:3000
```

> **Note:** Webcam access requires a secure context (`https://` or `localhost`). If opening via `file://`, the mouse fallback will be used automatically.

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Rendering | [Three.js r128](https://threejs.org/) — WebGL particle system |
| Hand Tracking | [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands) |
| Typography | [Syne](https://fonts.google.com/specimen/Syne) + [DM Mono](https://fonts.google.com/specimen/DM+Mono) |
| Build | None — single HTML file |

---

## 🪐 Formations

| Formation | Description |
|---|---|
| **Galaxy** | 5-arm spiral with core density gradient |
| **Nebula** | 6-lobe emission cloud with shifting hues |
| **Black Hole** | Accretion disc + polar jets + event horizon ring |
| **Saturn** | Layered ring bands with axial tilt |
| **Starship** | Cylindrical hull, nacelles, and engine exhaust plume |
| **Spacecraft** | Fuselage + delta wings + thruster glow |
| **DNA** | Double helix with rungs and strand colour coding |
| **Crystal** | Faceted multi-cluster growth |
| **Torus** | Torus knot (3,2) parametric curve |
| **Supernova** | Expanding shell + disc remnant + compact core |

---

## 📁 Project Structure

```
stellar/
├── index.html     # Entire engine — renderer, AI, UI, physics
└── README.md
```

---

## 🎛 Configuration

Key constants at the top of the script block in `index.html`:

```js
const COUNT   = 150000;  // Particle count — lower for slower devices
const DAMPING = 0.938;   // Velocity decay per frame
const SPRING  = 0.0065;  // Return-to-formation strength
```

---

## 📄 License

© 2025 [ayuuXploits](https://github.com/ayuuXploits). All Rights Reserved.

No part of this project — including source code, design, and assets — may be reproduced, distributed, modified, or used in any form without explicit written permission from the author.

---


Made with ✦ by <a href="https://github.com/ayuuXploits">ayuuXploits</a>
