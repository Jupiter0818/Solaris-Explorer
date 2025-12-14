# 🌌 Solaris Explorer: Final Edition

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Three.js](https://img.shields.io/badge/Three.js-r161-black) ![Status](https://img.shields.io/badge/Status-Completed-success)

**Solaris Explorer** 是一个基于 WebGL 的沉浸式 3D 宇宙探索模拟器。它利用 Three.js 和自定义着色器（GLSL）技术，构建了一个包含动态太阳系、深空天体和交互式 UI 的实时渲染环境。

**Solaris Explorer** is an immersive real-time 3D space simulation built with Three.js. It features a fully interactive solar system, procedural shaders, and cinematic visual effects.

## ✨ Key Features (核心功能)

* **🌞 Procedural Living Sun (动态活体太阳):** 使用自定义 Fragment Shader 实现的动态太阳表面，模拟日冕物质抛射和湍流效果。
* **🪐 Realistic Planet Rendering (拟真行星渲染):** 包含大气层散射（Atmosphere Shader）、动态云层、土星环以及拥有自发光纹理的城市夜景。
* **🌑 Volumetric Black Hole (体积光黑洞):** 模拟《星际穿越》风格的黑洞，包含吸积盘、引力透镜光子环和相对论喷流效果。
* **🌌 Deep Sky Objects (深空天体):** 交互式的旋涡星系（如仙女座 M31）和创生之柱（M16），全部由粒子系统构建。
* **🚀 Cinematic Travel (电影级穿越):** 实现了类似光速穿越的 "Warp Effect"（曲速引擎效果），伴随相机 FOV 的动态拉伸和后期光晕（Bloom）。
* **🛸 Voyager 1 Model (旅行者1号):** 精细建模的探测器，带有高光贴图和特定的运行轨道。
* **💻 Sci-Fi HUD Interface:** 玻璃拟态（Glassmorphism）风格的用户界面，实时显示天体数据、距离、温度和时间控制。

## 🛠️ Tech Stack (技术栈)

* **Core:** HTML5, CSS3 (Glassmorphism UI)
* **3D Engine:** [Three.js](https://threejs.org/) (v0.161 via ESM)
* **Post-Processing:** UnrealBloomPass (辉光效果)
* **Shaders:** Custom GLSL for Sun, Atmosphere, Black Hole accretion disk.
* **Math:** Geometry and physics simulations for orbital mechanics.

## 🚀 How to Run (如何运行)

由于项目使用了 ES Modules (`import` 语法) 和跨域资源，**不能直接双击打开 HTML 文件**。你需要一个本地服务器。

Since this project uses ES Modules, you need a local server to avoid CORS errors.

### Option 1: VS Code (Recommended)
1.  Install the **"Live Server"** extension in VS Code.
2.  Right-click `Galaxy.html` and select **"Open with Live Server"**.

### Option 2: Python
如果你安装了 Python，可以在项目目录下运行：
If you have Python installed, run this in your terminal:

```bash
# Python 3
python -m http.server 8000
