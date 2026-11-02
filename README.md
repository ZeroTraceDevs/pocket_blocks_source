# 🎮 POCKET BLOCKS — Dot Matrix Edition

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Build: Pure JS](https://img.shields.io/badge/Dependencies-None-brightgreen)
![Platform: Browser / Handheld](https://img.shields.io/badge/Platform-Web%20%7C%20Handheld-blue)
![ZeroTraceDevs Approved](https://img.shields.io/badge/Dev-ZeroTraceDevs-purple)

> **A retro-inspired falling-block puzzle game with a classic handheld look, modern display effects, gamepad support, and local save slots.**

---

### 📦 Quick Start & Ready-to-Play Download
Don't want to clone the repository? Simply grab the pre-packed release archive and launch the game instantly with a double-click:
* 💾 **[Direct Download: pocket_blocks_source.zip](https://github.com/ZeroTraceDevs/pocket_blocks_source/blob/main/pocket_blocks_source.zip)** *(Download, extract, and open `index.html`)*
* 🌐 **[Play Online via GitHub Pages](https://ZeroTraceDevs.github.io/pocket_blocks_source/)**

---

## 🌟 Overview
**POCKET BLOCKS** is a browser-based puzzle game inspired by the timeless charm of classic handheld gaming consoles. It combines a nostalgic dot-matrix aesthetic with modern web technologies, customizable display filters, full gamepad support, and reliable local save management.

The core mission of this open-source project by **ZeroTraceDevs** is to deliver an ultra-lightweight, accessible, and enjoyable retro gaming experience that runs directly in any modern web browser—completely free of installations, heavy frameworks, or cloud dependencies.

---

## ✨ Features in Detail

### 🕹️ Classic Gameplay
* **Authentic Mechanics:** Traditional falling-block puzzle gameplay featuring live tracking of scores, cleared lines, and difficulty levels.
* **Modern Quality-of-Life:** Upcoming-piece preview, piece-hold functionality, and ghost-piece positioning guides for strategic planning.
* **Flexible Input Methods:** Full keyboard controls, touch/on-screen buttons, and native **Gamepad API** integration for external controllers.

### 🖥️ Retro Display Experience & Shaders
* **Handheld Interface:** Beautifully styled console casing and retro layout.
* **Pixel-Perfect Canvas:** Fixed internal resolution of `200 × 180` pixels (maintaining a crisp 10:9 aspect ratio) to prevent layout distortion across modern displays.
* **Custom Display Modes & Filters:**
  * *Monochrome:* Classic handheld LCD aesthetic.
  * *OLED & Quantum Color:* Deep blacks, vivid saturation, and high contrast.
  * *ULED Simulation:* Emulated HDR contrast and local-dimming visual effects for a modern retro twist.
  *(Note: ULED and HDR options are browser-based aesthetic simulations and do not require or trigger physical hardware HDR specifications).*

### 💾 Local Save Management & JSON Export
* **Multi-Slot System:** Save and manage multiple game slots directly via browser `localStorage`.
* **JSON Backup:** Easily export or import your save data as a JSON file to transfer progress between devices or browsers.

### 🔊 Integrated Web Audio Synthesizer
* **Real-Time Sound Generation:** All sound effects are synthesized dynamically using the Web Audio API — **zero external audio files or MP3s required**.

### ⚡ Ultra-Lightweight (Performance First)
* **Pure Stack:** Built entirely with standard HTML5, CSS3, and vanilla JavaScript (ES6+).
* **Zero Bloat:** No external dependencies, no complex Node.js build steps on the client side. Perfectly optimized to run smoothly even on modest or legacy hardware (such as older Intel Pentium systems).

---

## 🎮 Controls & Key Bindings

| Action | Keyboard Input | Gamepad / Alternative |
| :--- | :--- | :--- |
| **Move Left / Right** | `Left / Right Arrow Keys` | D-Pad / Left Analog Stick |
| **Soft Drop** | `Down Arrow Key` | D-Pad Down |
| **Rotate Piece** | `Up Arrow Key` / `Z` / `X` | Action Buttons (A / B / X / Y) |
| **Hard Drop** | `Spacebar` | Top Action / Shoulder Button |
| **Hold Piece** | `C` / `Shift` | Left Bumper / Trigger |
| **Menu Navigation** | Mouse / Arrow Keys | D-Pad / Primary Buttons |

*Gamepad Note:* Connect any XInput or DirectInput compatible controller and press any button to allow the browser to register the device.

---

## 🚀 Installation & Getting Started

### Option 1: Run Locally (Standalone)
1. Download the [pocket_blocks_source.zip](https://github.com/ZeroTraceDevs/pocket_blocks_source/blob/main/pocket_blocks_source.zip) or clone the repository:
   ```bash
   git clone [https://github.com/ZeroTraceDevs/pocket_blocks_source.git](https://github.com/ZeroTraceDevs/pocket_blocks_source.git)
Ensure the core files reside in the same directory:index.htmlstyle.cssapp.jsDouble-click index.html to launch the game in your default web browser.Option 2: Host via GitHub PagesNavigate to your repository Settings > Pages.Set the Source to Deploy from a branch, choose your main branch, and select /root as the folder.Save your changes—GitHub will automatically publish your live web URL shortly.🛠️ Technology StackTechnologyPurposeHTML5Core structure and application markup containerCSS3Handheld frame styling, responsive layout, display filters & shadersJavaScript (ES6+)Game loop, collision detection, input mapping, and state machineHTML CanvasHigh-performance pixel-art rendering engineWeb Audio APIReal-time procedural sound effect generationWeb Storage / JSONLocal save persistence and data export/import formatting📁 Project StructurePlaintextpocket_blocks_source/
├── index.html               # Main entry point, UI structure, and canvas container
├── style.css                # Retro aesthetics, layout scaling rules, and shaders
├── app.js                   # Game engine, audio synth, input handler, and save manager
├── pocket_blocks_source.zip # Pre-packed ready-to-use archive for casual users
└── README.md                # Project documentation
💡 Feedback, Issues & ContributionsContributions and community feedback are always welcome! You do not need to be an expert developer to get involved:🐛 Report a Bug: Open an [suspicious link removed] detailing your browser version, operating system, and reproduction steps.🎨 Suggest Features: Recommend new color palettes, display filters, or accessibility improvements.🔧 Pull Requests: Keep changes clean, focused, and tested across multiple browser environments.🔒 PrivacyThe game runs 100% locally client-side. No telemetry data is collected, no external servers are tracked, and your save files stay safe and private inside your browser's local profile storage.❤️ Credits & LicenseCreated with passion by ZeroTraceDevs — dedicated to practical, high-performance, lightweight, and portable open-source software.Distributed under the MIT License. Check the LICENSE file for full terms.
