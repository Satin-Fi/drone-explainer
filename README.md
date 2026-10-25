# ASTRA AEROSPACE — Industrial Drone Explainer, Flight Simulator & Combat Arena

An interactive, web-based 3D industrial drone explainer, real-world flight simulator, and aerial combat arena built with **Three.js** and high-precision physics simulation.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-drone--explainer.vercel.app-00e5ff?style=for-the-badge&logo=vercel)](https://drone-explainer.vercel.app)
![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

🔗 **Live Production URL:** [https://drone-explainer.vercel.app](https://drone-explainer.vercel.app)

---

## 🌟 Key Features

### 1. 🔍 High-Fidelity CAD & Inside X-Ray Inspector
- **Aerospace Grade Composite Modeling**: Toray T700 carbon fiber frame, CNC aluminum motor clamps, and high-temperature neodymium outrunner BLDC motors.
- **0–100% Exploded View Slider**: Smoothly slides the top canopy, battery pack, avionics stack, gimbal camera, and motor arms outward along mechanical axes.
- **Inside X-Ray Mode**: Renders a translucent composite canopy revealing the internal STM32H7 flight controller, dual IMUs, 4-in-1 ESC, capacitor bank, and solid-state battery cells.
- **Interactive Component Hotspots**: Deep technical specs for Chassis, Avionics, Motors, Propellers, Battery, and LiDAR.

### 2. ✈️ 6-DOF Real-World Airspace Flight Simulator
- **Expansive Real-World Airspace**: Procedural sculpted terrain with rolling mountains, a 520-meter active runway with painted thresholds, airport terminal, control tower with rotating radar dish, 36 downtown glass skyscrapers, 220+ 3D trees, wind turbines, and flyable 3D cloud banks.
- **Smooth 6-DOF Flight Dynamics**: Direct heading-based velocity vectors, bank tilting, yaw turns, and an automatic barometric altitude-hold spring-damper.
- **Clean Full-Screen View**: Sidebars automatically collapse during flight into an aerospace telemetry OSD bar (Airspeed, Altitude, Battery, Health).

### 3. ⚔️ Aerial Combat Arena & Match Setup
- **Match Deployment Modal**:
  - **Play with Friends (Squad Co-Op)**: Deploy alongside 2 Allied Wingmen (*Viper-2* & *Ghost-4*) flying in echelon formation, assisting with laser fire and tactical radio transmissions.
  - **Single Player (Solo Ace)**: Take on the hostile drone swarm alone.
- **Audio & Radio Controls**:
  - Master Sound & Weapon FX (`ON` / `OFF`) via procedural Web Audio synthesizer.
  - Tactical Radio Chatter & killfeed alerts (`ON` / `OFF`).
- **Swarm Threat Levels**: Cadet (3 enemies), Veteran (5 enemies), or Incursion (8 enemies).
- **Weapons & Armory**: Dual Pulse Lasers, Homing Missiles with exhaust trails, EMP blast wave, and magnetic coin collection (+50 / +150 combo popups).

### 4. 📹 Camera Director & Angle Controls Dock
- **8 Dynamic Camera Modes**:
  1. **Chase** (3rd-Person Tactical with heading lag)
  2. **FPV Cockpit** (First-person nose gimbal view with horizon tilt)
  3. **Action Cam** (Aggressive close-tail follow cam)
  4. **Top-Down Recon** (32m satellite bird's-eye view)
  5. **Wingman Cam** (Profile side flight view)
  6. **Front Reverse** (Nose-in looking back at the drone)
  7. **Cinematic 360°** (Continuous smooth orbit showcase)
  8. **Free Orbit** (360° manual mouse/touch orbit & zoom anytime)
- **7 Angle Presets**: Rear (0°), Front (180°), Port (-90°), Starboard (+90°), Top (85°), ISO (3/4), Underbelly (-35°), plus instant **Flip 180°** (`V`).
- **Live Sliders**: Distance / Zoom (`2m` - `22m`), Vertical Tilt (`-35°` - `+35°`), and FOV (`45°` - `95°`).

---

## 🎮 Flight & Combat Controls

| Action | Keyboard | Touch / Mouse Controls |
| :--- | :--- | :--- |
| **Cruise / Move** | <kbd>W</kbd> <kbd>S</kbd> | Left Virtual Joystick |
| **Strafe / Turn** | <kbd>A</kbd> <kbd>D</kbd> | Left Virtual Joystick |
| **Yaw / Heading** | <kbd>Q</kbd> <kbd>E</kbd> | Right Virtual Joystick |
| **Climb / Descend** | <kbd>SPACE</kbd> / <kbd>SHIFT</kbd> | Dedicated `▲` / `▼` Altitude Buttons |
| **Dual Pulse Lasers** | **Left-Click** or <kbd>F</kbd> | `LASER` Action Button |
| **Homing Missiles** | **Right-Click** or <kbd>M</kbd> | `MISSILE` Action Button |
| **Cycle Camera Mode** | <kbd>C</kbd> | `📹 CAM` Button / OSD Dropdown |
| **Flip Camera 180°** | <kbd>V</kbd> | Camera Director Flip Button |
| **Direct Camera Modes** | Keys <kbd>1</kbd> – <kbd>8</kbd> | Camera Director Mode Chips |
| **Match Setup Modal** | **⚙️ Match Setup** | OSD Action Button |
| **Respawn / Center** | <kbd>R</kbd> | `↺ Respawn` Button |

---

## 🚀 Getting Started

### Local Preview
Simply open `index.html` or `drone-explainer.html` in any modern web browser:

```bash
# Using Python
python -m http.server 3000

# Using Node.js
npx serve .
```

Open [http://localhost:3000](http://localhost:3000) to launch the simulation.

---

## 🛠️ Tech Stack

- **Three.js** (WebGL 3D Rendering & Shaders)
- **Web Audio API** (Procedural multi-oscillator turbine engine, laser plasma, missile thruster & explosion synthesizer)
- **Vanilla HTML5 & CSS3** (Astra porcelain glassmorphism design system)
- **Vercel** (Cloud deployment & global edge CDN)

---

## 📜 License

MIT License. Designed and developed for Astra Aerospace.
