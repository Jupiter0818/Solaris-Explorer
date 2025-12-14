# 🌌 Solaris Explorer: Final Edition

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Three.js](https://img.shields.io/badge/Three.js-r161-black) ![Status](https://img.shields.io/badge/Status-Completed-success)

<p align="center">
  <img src="assets/main-banner.gif" width="100%" alt="Solaris Demo">
</p>

**Solaris Explorer** is an immersive, real-time 3D universe simulation built purely with **Three.js** and **WebGL**. 

This project pushes the boundaries of browser-based rendering, featuring procedural living stars, volumetric black holes inspired by *Interstellar*, and cinematic warp-speed travel effects—all running smoothly in a standard web browser.

## ✨ Key Features

* **🌞 Procedural Living Sun**
    * Utilizes custom **Fragment Shaders (GLSL)** to simulate a dynamic photosphere with turbulence and coronal mass ejections.
    * Features physically based glow and noise-driven surface generation.

* **🪐 Realistic Planetary Rendering**
    * **Atmospheric Scattering:** Implements custom shaders for realistic atmospheric halos on Earth, Venus, and Mars.
    * **Saturn's Rings:** Simulates ring systems using tens of thousands of individual particles.
    * **Voyager 1 Model:** Includes a high-fidelity 3D model of the probe with its iconic Golden Record.

* **🌑 Volumetric Black Hole**
    * A stunning visual simulation of a supermassive black hole.
    * Features a **volumetric accretion disk**, gravitational lensing (photon ring), and relativistic jets.

* **🌌 Deep Sky Objects**
    * **Interactive Galaxies:** Spiral galaxies (like Andromeda M31) built with particle systems that support dynamic rotation and color gradients.
    * **Pillars of Creation (M16):** Volumetric cloud rendering to recreate the famous nebula structures.

* **🚀 Cinematic Experience**
    * **Warp Drive:** Seamless "Light Speed" travel effect with dynamic FOV (Field of View) stretching and spatial distortion.
    * **Sci-Fi HUD:** A fully functional, glassmorphism-styled User Interface displaying real-time telemetry, temperature, and astronomical data.

## 🛠️ Tech Stack

* **Core Engine:** [Three.js](https://threejs.org/) (r161, via ES Modules)
* **Languages:** HTML5, CSS3, JavaScript (ES6+)
* **Rendering:** * WebGL 2.0
    * **Post-Processing:** UnrealBloomPass, EffectComposer
    * **Shaders:** Custom GLSL for the Sun, Black Hole, and Atmosphere.
* **Physics:** Orbital mechanics and particle simulations.

## 🚀 How to Run

⚠️ **Note:** Because this project uses **ES Modules** (`import`) and cross-origin textures, it **cannot** be run by simply double-clicking the HTML file. You must use a local server.

### Option 1: VS Code (Recommended)
1.  Install the **"Live Server"** extension in VS Code.
2.  Right-click `index.html` (or `Galaxy.html`).
3.  Select **"Open with Live Server"**.

### Option 2: Python
If you have Python installed, open your terminal in the project folder and run:

```bash
# Python 3
python -m http.server 8000
