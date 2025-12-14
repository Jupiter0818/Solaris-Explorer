# 🌌 Solaris Explorer: Final Edition

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Three.js](https://img.shields.io/badge/Three.js-r161-black) ![Status](https://img.shields.io/badge/Status-Completed-success)

**Solaris Explorer** 是一个基于 WebGL 的沉浸式 3D 宇宙探索模拟器。该项目利用 Three.js 和自定义 GLSL 着色器技术，在浏览器中构建了一个包含动态太阳系、体积光黑洞、深空天体以及电影级视觉效果的实时渲染环境。

## ✨ 核心亮点

* **🌞 动态拟真太阳 (Procedural Living Sun):**
    * 使用自定义 Fragment Shader（片元着色器）实现动态的太阳表面，模拟真实的日冕湍流和热辐射效果。
    * 包含日冕辉光（Bloom）与基于噪声算法的表面纹理生成。

* **🪐 逼真的行星渲染:**
    * **大气散射：** 为地球、金星、火星等行星实现了基于物理的大气层光晕（Atmosphere Shader）。
    * **土星环与卫星：** 使用数万个粒子模拟土星环，并精确还原了各大行星的主要卫星轨道。
    * **旅行者1号 (Voyager 1):** 内置高精度的旅行者1号探测器 3D 模型，带有反光材质与独特的金色唱片结构。

* **🌑 《星际穿越》风格黑洞:**
    * 实现了体积光吸积盘（Volumetric Accretion Disk）与引力透镜效果。
    * 包含相对论喷流与事件视界（Event Horizon）的视觉模拟。

* **🌌 交互式深空天体:**
    * **粒子星系：** 数万个粒子构成的旋涡星系（如仙女座 M31），支持动态旋转与色彩渐变。
    * **创生之柱 (M16):** 使用体积云粒子技术重现了壮观的星云结构。

* **🚀 电影级体验:**
    * **曲速穿越 (Warp Effect):** 实现了点击天体后的光速穿越特效，伴随相机视场角（FOV）拉伸与空间扭曲。
    * **科幻 UI 界面:** 采用玻璃拟态（Glassmorphism）设计风格，实时显示天体距离、速度、温度等遥测数据。

## 🛠️ 技术栈

* **核心引擎:** [Three.js](https://threejs.org/) (r161, 基于 ESM 模块)
* **语言:** HTML5, CSS3, JavaScript (ES6+)
* **渲染技术:** * WebGL 2.0
    * Post-Processing (后期处理): UnrealBloomPass (辉光), EffectComposer
    * GLSL Shaders (自定义着色器)
* **数学库:** 轨道力学模拟与 3D 向量计算

## 🚀 如何运行项目

⚠️ **注意**：本项目使用了 ES Modules (`import` 语法) 和跨域纹理资源，**无法直接双击 HTML 文件打开**，必须在本地服务器环境下运行。

### 方法 1：使用 VS Code (推荐)
1.  在 VS Code 中安装 **"Live Server"** 扩展插件。
2.  右键点击 `index.html` (或 `Galaxy.html`)。
3.  选择 **"Open with Live Server"**。

### 方法 2：使用 Python
如果您已安装 Python 环境，可在项目根目录下运行终端命令：

```bash
# Python 3
python -m http.server 8000
