# 🎮 POCKET BLOCKS — Dot Matrix Edition

**A retro-inspired falling-block puzzle game with a classic handheld look, modern display effects, gamepad support, and local save slots.**

POCKET BLOCKS is a browser-based puzzle game inspired by the charm of classic handheld gaming devices. It combines a nostalgic dot-matrix aesthetic with modern browser technologies, customizable display effects, keyboard and gamepad controls, and convenient local save management.

The goal of the project is simple: create a lightweight, accessible, and enjoyable retro gaming experience that runs directly in a web browser without requiring an installation, a server, or external JavaScript libraries.

This project is a work in progress, and community feedback, bug reports, ideas, and contributions are always welcome!

---

## ✨ Features

### 🕹️ Classic Gameplay
- Falling-block puzzle gameplay inspired by classic arcade and handheld games.
- Score, cleared lines, and level tracking.
- Upcoming-piece preview and piece-hold functionality.
- Ghost-piece preview to help plan placements.
- Keyboard controls and on-screen buttons.
- Gamepad support through the browser's Gamepad API.

### 🖥️ Retro Display Experience
- A handheld console-inspired interface.
- Pixelated rendering for a classic dot-matrix appearance.
- Multiple display color modes, including monochrome-inspired and modern color palettes.
- Visual display filters designed to reproduce different screen characteristics.
- OLED-inspired color presentation and vivid color options.
- ULED-inspired visual effects, including vivid color, HDR-style contrast, and local-dimming-style effects.

**Note:** ULED, HDR, and local-dimming options are visual simulations implemented in the browser. They do not activate physical display hardware or provide genuine hardware HDR.

### 💾 Local Save Management
- Multiple local save slots.
- Save data stored in the browser using `localStorage`.
- JSON export and import for transferring or backing up supported game data.

Save data is stored locally in the current browser profile. Clearing browser data or using a different browser may affect access to existing saves.

### 🔊 Audio
- Browser-generated sound effects using the Web Audio API.
- No external audio files required.

### ⚡ Lightweight by Design
- Built with standard HTML, CSS, and JavaScript.
- No installation or build step required for the basic local version.
- No external framework required.
- Designed to remain lightweight and run on modest computer hardware.

Actual performance depends on the browser, operating system, and hardware.

---

## 📖 How the Project Started

POCKET BLOCKS began with a simple idea: recreate the feeling of playing a small, classic handheld puzzle game while keeping the experience easy to access on modern computers.

Instead of building a large game engine or relying on a complex framework, the project uses familiar web technologies. The interface takes inspiration from physical handheld consoles, while the game itself uses a small pixel-based canvas.

As the project developed, the original idea grew into something more ambitious. Display customization, controller support, local save slots, data export, and additional quality-of-life features became part of the concept.

One important part of the development process has been refining the display scaling. A pixel-based game should preserve its intended aspect ratio when resized, rather than stretching the playfield or making the blocks look distorted. This is an ongoing area for testing and improvement across different screen sizes and browsers.

POCKET BLOCKS is built around experimentation, practical improvements, and the idea that a small browser game can still offer a surprisingly customizable experience.

---

## 🚀 Getting Started

### Option 1: Run Locally

1. Download or clone this repository.
2. Make sure the following files are in the same directory:
   - `index.html`
   - `style.css`
   - `app.js`
3. Open `index.html` in a modern web browser.
4. Start a game and try the available display settings and controls.

No package installation or compilation should be necessary for the basic version.

### Option 2: Run Through GitHub Pages

You can publish the project as a static website using GitHub Pages:

1. Upload the project files to a GitHub repository.
2. Open the repository's **Settings**.
3. Select **Pages**.
4. Choose the branch you want to publish and the appropriate folder, usually `/ (root)`.
5. Save the settings and wait for GitHub Pages to publish the site.

The resulting website URL will be shown in the Pages settings.

---

## 🎮 Controls

The exact controls depend on the current implementation and browser support.

| Action | Input |
|---|---|
| Move left or right | Arrow keys or on-screen directional controls |
| Move down | Down arrow |
| Rotate a piece | Configured action key or on-screen button |
| Hard drop | Configured action key |
| Hold a piece | Configured hold key or button |
| Navigate menus | Mouse, keyboard, or supported controller inputs |

**Gamepad:** Connect a compatible controller before or during gameplay. Support depends on the browser and controller mapping. Some browsers require a button press before making a controller available to the page.

For the exact key bindings, consult the current JavaScript implementation.

---

## 🖼️ Display Scaling and Filters

The game uses a small internal canvas to preserve its pixel-art character.

The intended internal display resolution is **200 × 180 pixels**, giving it a **10:9 aspect ratio**.

When changing the size of the display, the goal is to preserve this ratio and avoid stretching the game vertically or horizontally. CSS controls the visible size, while the canvas provides the internal drawing surface.

The display options explore several visual styles:

- **Monochrome:** A classic handheld-inspired appearance.
- **Color:** A more colorful presentation.
- **OLED-inspired:** Deep blacks and strong contrast.
- **Quantum Color-inspired:** A vivid, saturated palette.
- **ULED-inspired effects:** Simulated HDR-style contrast, vivid colors, and local-dimming-style presentation.

These effects are aesthetic approximations rather than accurate simulations of every physical display technology.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Game structure and interface |
| CSS3 | Handheld styling, responsive layout, display modes, and filters |
| JavaScript | Gameplay, input handling, and application logic |
| HTML Canvas | Pixel-based game rendering |
| Web Audio API | Generated sound effects |
| Gamepad API | Compatible game controller input |
| Local Storage | Local save data |
| JSON | Save export and import |

The project is intended to remain easy to inspect, modify, and extend without a large development environment.

---

## 📁 Project Structure

```text
pocket-blocks/
├── index.html    # Main page and game interface
├── style.css     # Visual design and display scaling
├── app.js        # Game logic, controls, and save management
└── README.md     # Project documentation
```

The exact repository may contain additional files as the project evolves.

---

## 🧪 Testing and Current Development

POCKET BLOCKS is a developing project, so testing on different systems is important.

Areas worth checking include:

- Display scaling on different resolutions and browser zoom levels.
- Correct canvas aspect ratio and pixel rendering.
- Keyboard controls and controller compatibility.
- Save-slot behavior and JSON import/export.
- Display filters and their performance impact.
- Gameplay responsiveness on older computers.
- Layout behavior on smaller screens.

Not every browser, controller, or hardware configuration has been verified. Please report issues with as much useful detail as possible.

---

## 💡 Feedback and Contributions

**Your feedback is welcome!**

POCKET BLOCKS can improve through community testing, ideas, bug reports, and contributions. You do not need to be an experienced developer to help.

### Ways to contribute

- Report bugs or unexpected behavior.
- Suggest new display modes or visual effects.
- Recommend improvements to the handheld interface.
- Test the game with different controllers and browsers.
- Identify performance problems or scaling issues.
- Suggest gameplay improvements and accessibility options.
- Contribute code, documentation, or testing notes.

### Reporting a bug

When opening an issue, please include:

1. A short description of the problem.
2. The steps needed to reproduce it.
3. Your browser and operating system.
4. Your screen resolution, if the issue concerns scaling.
5. The controller model, if the issue concerns gamepad input.
6. Any relevant screenshots or console errors.

### Suggesting a feature

Please explain what you would like to see, why it would be useful, and how you imagine it working. Clear, constructive suggestions are especially helpful.

For code contributions, keep changes focused, preserve existing functionality where possible, and explain what you changed and how you tested it.

---

## 🔒 Privacy

The game is designed to run locally in the browser without requiring an account or a backend server.

Save data is kept in browser storage. Exported JSON files may contain game data, so review them before sharing.

The project should not be assumed to provide network-free operation in every deployment environment without checking the actual code and hosting setup.

---

## 🗺️ Roadmap Ideas

Potential areas for future development include:

- [ ] More display palettes and customizable filter settings.
- [ ] Improved scaling across different aspect ratios and window sizes.
- [ ] More extensive controller configuration.
- [ ] Additional sound and accessibility options.
- [ ] More robust save-data validation and recovery.
- [ ] Automated gameplay and input tests.
- [ ] Performance profiling on older hardware.
- [ ] Expanded documentation and screenshots.

This list is a collection of ideas, not a promise that every feature is already implemented or scheduled.

---

## 📜 License

A license has not been specified here. Before reusing, modifying, or redistributing this project, check the repository for a `LICENSE` file. If you are the project owner, consider adding an appropriate open-source license to make the intended permissions clear.

---

## ❤️ Thank You

Thank you for checking out POCKET BLOCKS — Dot Matrix Edition!

The project is about bringing a little of the classic handheld gaming experience into the browser while leaving room for experimentation and improvement.

If you try it, find a bug, have an idea, or want to help make it better, feedback is greatly appreciated.

**Have fun, enjoy the pixels, and happy gaming!** 🎮
