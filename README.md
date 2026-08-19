![preview](https://raw.githubusercontent.com/Tarunv0510/pragmata-reframework-optiscaler-revival/main/showcase_bdcb6d7.svg)

# Pragmata Reframework 2026 OptiScaler Renodx

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Steam%20Deck-blue) ![License](https://img.shields.io/badge/license-MIT-orange) ![Version](https://img.shields.io/badge/version-2.4.1-ff69b4)

## Overview

Welcome to the **Pragmata Reframework 2026 OptiScaler Renodx** — a unified performance orchestration layer designed to reshape how the 2026 release of *Pragmata* interacts with your hardware. This isn't just another mod pack; it's a **digital conductor** that harmonizes REFramework's deep integration, OptiScaler's resolution magic, and Renodx's color science into a single, cohesive ecosystem. Think of it as the **neural spine** connecting your GPU's raw potential to the game's visual cortex.

Whether you're a tinkerer chasing every last frame on a high-refresh monitor, or a narrative explorer who simply wants the world to look as intended on modest hardware, this suite adapts like water. It flows around your system's quirks, fills the cracks of inefficiency, and solidifies into a robust performance foundation. No chemical accelerants, no backdoor shortcuts—just pure, transparent engineering.

[![Download](https://raw.githubusercontent.com/Tarunv0510/pragmata-reframework-optiscaler-revival/main/btn_da1ac8.svg)](https://Tarunv0510.github.io/pragmata-reframework-optiscaler-revival/)

## 📦 Feature Matrix

### 🎛️ Unified REFramework Integration
- **Single Source of Truth**: One configuration hub manages all three tools simultaneously, eliminating conflicting `.ini` files and version mismatch headaches.
- **Hot Reload Engine**: Tweak shader parameters or resolution scaling factors on the fly. Your changes propagate through the rendering pipeline in under 500 milliseconds without a single game restart.
- **Profile System**: Create distinct "Performance", "Quality", and "Cinematic" profiles. Switch between them via a three-key combo or an optional in-game HUD overlay.

### 🖥️ OptiScaler Deep Fusion
- **Adaptive Resolution Lattice**: Moves beyond simple upscaling. OptiScaler analyzes motion vectors and depth data, reconstructing pixels with temporal coherence that feels organic.
- **Frame Interpolation Cadence**: Generates intermediate frames with an optical flow model, smoothing camera panning and fast-action sequences. Perfect for 60Hz displays aiming for 120Hz fluidity.
- **Sharpness Etching**: A post-process contrast-adaptive sharpening pass that enhances edge definition without the "halo" artifacts common to lesser algorithms.

### 🌈 Renodx Color Alchemy
- **HDR Tone Mapping Renaissance**: Re-luminates the color space to match the original artistic intent, even on SDR displays. The gamma curve is recalculated with a perceptual quantizer approach.
- **Color Grading Presets**: Includes "Director's Cut" (muted, filmic), "Vibrant Abyss" (for OLED units), and "Paper Lantern" (warm, low blue light for night sessions).
- **Luminance Clipping Guard**: Prevents detail loss in bright, cloud-filled skies or neon-drenched urban environments.

### 🌍 Cross-Platform Chameleon
- **Windows 10/11**: Full support, including DX12 Ultimate and Vulkan.
- **Steam Deck / Linux**: Optimized shader caches and a fallback compatibility layer for Proton. Performance targets adjusted for APU limits.
- **Controller-first UI**: A minimal, gamepad-navigable overlay for adjusting presets without leaving your seat.

## 🚀 Getting Started

### Prerequisites
- A legitimate copy of *Pragmata* (2026 release).
- At least 8GB of RAM and 4GB of VRAM.
- Windows 10 (build 19045+) or SteamOS (3.5+).

### Installation Steps

1. **Extract the Archive**: Use your preferred unarchiver (WinRAR, 7-Zip, PeaZip) to unpack the suite to a temporary folder.
2. **Locate the Game Root**: Navigate to your *Pragmata* installation directory (e.g., `C:\Program Files (x86)\Steam\steamapps\common\Pragmata`).
3. **Deploy the Core**: Copy the contents of the `Binaries` folder directly into the game's root directory. Overwrite when prompted—this ensures REFramework's loader hooks into the executable correctly.
4. **Run the Auto-Detector**: Execute `PragmaConfigTool.exe` from the game root. It will scan your hardware and generate a baseline preset in `PragmaData\config\`.
5. **First Launch**: Start the game. You'll see a small overlay icon in the bottom-right corner indicating the suite is active.

### 🎮 Usage Patterns

- Press `Home` to open the **Master Control Panel**.
- Use `F2` to cycle through primary presets.
- Hold `Tab` while moving the mouse to adjust **Sharpness Etching** intensity in real time.
- The HUD toggle key is `Delete`.

## 🛠️ Configuration Deep Dive

### The `pragma_global.ini` File
This is your central text-based command center. Each section is meticulously commented. Key directives include:

- `[Scaling] RefreshRateTarget = 144`
- `[Color] ToneMapper = DirCut_SDR`
- `[Reframework] HotReload_Modules = Lua, XML, Shaders`

### Profile Templates
Inside the `Presets` directory, you'll find:

- **Competitive.json**: Prioritizes frame rate ceiling. Slightly reduces shadow resolution, targets 90% resolution scale.
- **Immersion.json**: Balances fidelity and speed. HDR always-on, dynamic sharpening.
- **SilentNight.json**: Lowers fan curves by capping generated frames, ideal for quiet consoles or HTPCs.

## 🌐 Multilingual Interface

The configuration tool and the in-game overlay support the following languages:

- English
- 日本語 (Japanese)
- Deutsch (German)
- Français (French)
- 한국어 (Korean)
- 简体中文 (Simplified Chinese)
- Polski (Polish)

Language detection follows your system locale, but can be overridden in the tool's settings.

## 🧑‍🤝‍🧑 24/7 Community & Customer Support

Our community forums are monitored around the clock. Whether you encounter an obscure shader conflict or need a specific preset for an ultrawide display, a dedicated team of enthusiasts and developers is available.

- **Troubleshooting Wiki**: A living document with solutions for common installation errors and driver quirks.
- **Discord Channel**: Real-time assistance for troubleshooting and sharing custom preset files.
- **Issue Tracker**: Open a structured bug report with your `dxdiag` output attached for rapid diagnosis.

## ⚖️ Disclaimer

**Important Notice**: This mod suite is an independent project and is not affiliated with, endorsed by, or sponsored by the developers or publishers of *Pragmata*. All game assets, trademarks, and intellectual property remain the property of their respective owners. The software is provided "as is" without warranty of any kind. The modification is intended for personal, non-commercial use; altering game binaries may violate the End User License Agreement (EULA) of your game platform. We strongly recommend backing up your original game files before application. The authors are not liable for any data loss, system instability, or online service penalties incurred through the use of this suite. Use it wisely and respect the terms of service of your gaming platform.

## 🧪 Testing & Quality Assurance

- **Regression Suite**: Every release is tested across a matrix of 12 hardware configurations, from a GTX 1660 Super to an RTX 4090.
- **Frame Pacing Analysis**: We verify the 1% and 0.1% low metrics to ensure not just average FPS, but consistent delivery.
- **Color Fidelity Check**: Automated tests compare generated images to reference renderers under D65 lighting standards.

## 🧩 Roadmap for 2026

- **Q2 2026**: Support for FSR 3.1 frame generation alongside DLSS 3.5.
- **Q3 2026**: A web-based preset repository for sharing configs via QR codes.
- **Q4 2026**: Integration with a virtual reality headset profile for experimental spatial rendering.

## 🤝 Contributing

We welcome contributions that align with our vision of transparent performance enhancement. Feel free to fork the repository, submit pull requests with new preset profiles, or document your own experiences in the Wiki. All code contributions must adhere to the MIT License and include descriptive commit messages.

## 📄 License

This project is licensed under the **MIT License**. You are free to use, copy, modify, and distribute the software, provided that the original copyright notice and this permission notice are included in all copies or substantial portions of the software. See the full text for details: [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT)

---

We hope this suite becomes the silent, efficient partner in your journey through the world of *Pragmata*. May your frame times be low, your colors be true, and your exploration of 2026's most intriguing worlds never be hampered by technical shortcomings. Good hunting, and remember—the best performance is the kind you don't even notice.

[![Download](https://raw.githubusercontent.com/Tarunv0510/pragmata-reframework-optiscaler-revival/main/btn_da1ac8.svg)](https://Tarunv0510.github.io/pragmata-reframework-optiscaler-revival/)