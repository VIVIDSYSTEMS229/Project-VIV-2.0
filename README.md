# Project-VIV-2.0
Custom-calibrated graphics pipeline and engine memory framework for GTA V Enhanced. Bypasses 30 FPS framework caps, mitigates ERR_GFX_STATE crashes under heavy VRAM loads, and eliminates blinding overexposures via tuned RenoDX/ReShade structures. Made by VIVID Systems.
# PROJECT VIV — Next-Gen Photorealism & Engine Fix for GTA V Enhanced

Welcome to the Leonida Prep-Phase. **Project VIV** is officially live.

Building, testing, and optimizing a true next-generation graphical overhaul over the native Enhanced engine architecture is a massive undertaking. It required a significant amount of deep configuration, log monitoring, and engine calibration to get the exposure, stability, and memory pooling exactly right. It was a massive amount of work, but it is an absolute blast to do from a developer's perspective.

This project delivers a precision-calibrated visual experience, balanced contrast mapping via custom RenoDX HDR/SDR pipelines, and manual memory optimization variables designed to let high-end hardware perform exactly the way it was meant to—completely free of engine bottlenecks and rendering anomalies.

---

## 🚀 Key Features

* **Engine Stability & Memory Fix:** Built-in memory adjusters and pooling variables to completely mitigate standard rendering crashes (`ERR_GFX_STATE`) under heavy VRAM loads.
* **Bypassed Performance Caps:** Fully eliminates double-buffering framework bottlenecks during borderless windowed operation.
* **Balanced Light Exposure:** Custom-calibrated tone-mapping (via the 'onigiri' layout) to completely remove blinding overexposure and blown-out whites at Rockford Plaza.
* **Crisp Fidelity:** Disabled aggressive camera motion ghosting to preserve raw texture sharpness in high-speed motion.

---

## 📊 System Requirements

### Developer Testing Rig (Baseline Calibration)
* **CPU:** Intel Core i7-14700K
* **GPU:** AMD Radeon RX 9070 XT 
* **RAM:** 24GB DDR4
* **VRAM Allocation:** Real-world game usage is stable around ~10GB VRAM.

### Target Hardware for Testers
* **OS:** Windows 10 / 11 (64-bit)
* **Processor (CPU):** Intel Core i5-10400 / i5-10600 (10th Gen) or AMD Ryzen 5 3600 / 5500 equivalent
* **System RAM:** 16GB Minimum
* **Storage:** SSD Required (Crucial for streaming high-resolution assets without pop-in)
* **Graphics Card (GPU with min. 12GB VRAM):**
  * **AMD:** Radeon RX 6700 XT / RX 7700 XT (12GB) or higher
  * **NVIDIA:** GeForce RTX 3060 (12GB) / RTX 4070 (12GB) or higher

---

## ⚙️ Mandatory Launch Options

To ensure the custom graphics engine and scripts load correctly without anti-cheat interference, you **MUST** paste the following parameter into your game launcher (Steam / Rockstar Launcher) properties before launching:

```text
-nobattleye
```

---

## 🛠️ Installation & Calibration Guide

### Step 1: File Deployment
1. Ensure you have a clean copy of GTA V Enhanced with **ScriptHookV** and **ASI Loader** installed via OpenIV. 
2. Make sure the `-nobattleye` flag is active in your launch options.
3. Extract the contents of the provided `.rar` archive directly into your main GTA V directory (where `GTA5.exe` is located). Replace files if prompted.

### Step 2: Critical In-Game Configuration
To achieve the exact photorealistic output baseline, you must calibrate your in-game menus to the absolute maximum fidelity available:

* **Brightness Calibration:** Go to *Settings -> Display* and set your **Brightness slider to exactly 50% (dead center)**. This is crucial—the RenoDX tone-mapping layer relies entirely on a neutral system baseline to balance exposures correctly.
* **Unshackle the Visuals (Maximum Ultra Settings):** Go to *Settings -> Graphics* and push the engine to its absolute limits. You **MUST** change all texture, shader, shadow, water, particle, reflection, and grass quality settings to the **highest possible options available in the game (Ultra / Very High)**. 
* **Limiter Warnings:** Keep **MSAA turned OFF** and ensure the native **Frame Generation toggle remains disabled** to prevent framework rendering conflicts.

---

## 💬 Community Testing & Feedback

We are looking for feedback on cross-compatibility, frame pacing, and lighting behavior across different monitors. If you experience an unexpected crash, please submit an **Issue** with your hardware specifications and your `Launcher.log` attached.

*Developed by VIVID Systems.*
