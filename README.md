# ASTRA AEROSPACE — Industrial Drone Explainer & Flight Simulator

An interactive, web-based 3D industrial drone explainer, real-world flight simulator, and aerial combat arena built with **Three.js** and high-precision physics simulation.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-drone--explainer.vercel.app-00e5ff?style=for-the-badge&logo=vercel)](https://drone-explainer.vercel.app)
![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

🔗 **Live Production URL:** [https://drone-explainer.vercel.app](https://drone-explainer.vercel.app)

---

## 🌟 Key Features

- **High-Fidelity 3D Drone Model**:
  - Carbon fiber frame with matte coating and realistic structural arms
  - High-torque brushless motors with spinning propeller discs and dynamic lift particles
  - 3-axis stabilized 4K gimbal camera with dual-lens optical system & protective sensor ring
  - LiDAR puck sensor, GPS mast with illuminated status rings, and dual battery bays
  - Full lighting system: Navigation LEDs (Red port, Green stbd, White tail strobe), searchlights, and battery indicator bars
- **Interactive Explainer & Hotspots**:
  - Interactive clickable hotspots for key sub-systems (Propulsion, Avionics & LiDAR, Camera Gimbal, Power System)
  - Detailed technical breakdowns and specifications for each subsystem
  - Subsystem highlight & inspection modes with smooth camera focus transitions
- **Real-World Flight Physics Simulator**:
  - Realistic quadcopter flight dynamics (Pitch, Roll, Yaw, Collective Thrust)
  - Inertia, aerodynamic drag, angular momentum, and ground collision detection
  - Keyboard & interactive HUD controls (Throttle, Steering, Hover Lock, Return-To-Home)
  - Dynamic wind vector simulation with configurable speed and turbulence
  - Altitude, velocity, climb rate, and compass instrumentation overlays
- **Modern Industrial UI**:
  - Dark-mode glassmorphic HUD with telemetry displays and flight graphs
  - Responsive design optimized for desktop and mobile displays
  - Zero build step required — runs directly in modern browsers via vanilla HTML5, CSS3, and Three.js

---

## 🎮 Flight Controls

| Action | Keyboard | HUD Controls |
| :--- | :--- | :--- |
| **Throttle Up (Climb)** | `W` or `Arrow Up` | Dedicated Vertical Slider / Button |
| **Throttle Down (Descent)** | `S` or `Arrow Down` | Dedicated Vertical Slider / Button |
| **Yaw Left (Rotate Left)** | `A` or `Arrow Left` | Rudder Slider / Left Pad |
| **Yaw Right (Rotate Right)**| `D` or `Arrow Right`| Rudder Slider / Right Pad |
| **Pitch & Roll (Translate)**| `I` / `K` / `J` / `L` | Virtual Joystick Pad |
| **Hover Lock (Auto-Level)**| `Space` | "Hover Lock" Toggle |
| **Return to Home (RTH)** | `H` | "RTH" Button |
| **Toggle Explainer / Flight Mode** | UI Switcher | Mode Selector Bar |

---

## 🚀 Getting Started

### Local Preview
Simply open `index.html` in any modern web browser, or use a local HTTP server:

```bash
# Using Python
python -m http.server 3000

# Using Node.js npx
npx serve .
```

Open [http://localhost:3000](http://localhost:3000) to view the simulator.

---

## 🛠️ Tech Stack

- **Three.js** (WebGL 3D Rendering)
- **OrbitControls** (Camera inspection manipulation)
- **HTML5 & CSS3 Custom Properties** (Futuristic aerospace glassmorphic UI)
- **Vanilla JavaScript** (Physics engine, vector math, telemetry computation)
- **Vercel** (Cloud deployment & edge CDN hosting)

---

## 📜 License

MIT License. Designed and developed for Astra Aerospace.
