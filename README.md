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

### 2. ✈️ 5,000-Meter Tactical Battlefield Airspace
- **Expansive 5km Airspace Across 5 Sectors**:
  - **Sector 1 (Center): Alpha Military Airbase**: 1,200-meter dual runway, parallel taxiways, 4 massive aircraft hangars, SAM missile defense battery, control tower with radar dish, and twin helipads.
  - **Sector 2 (East): Cyber Megalopolis Skyline**: 80+ skyscrapers (up to 260m high) with skybridges, illuminated rooftop helipads with coins, and red aviation hazard beacons.
  - **Sector 3 (South): Industrial Petrochemical Complex**: 4 hyperbolic cooling towers, 8 spherical fuel storage tanks, 6 flare stacks with flame effects, and pipeline corridors.
  - **Sector 4 (West): Naval Harbor & Aircraft Carrier**: Deep ocean basin with a 320-meter Aircraft Carrier battleship (flight deck with catapult lines & island command tower), escort frigates, and an offshore deep-sea platform with helipad.
  - **Sector 5 (North): Alpine Mountain Ridgeline**: Towering mountain passes (up to 240m elevation), flight canyons, 12 giant wind turbines, and 500+ trees.
- **Battlefield Perimeter Warning**: Airspace containment zone (2,400m radius) with "LEAVING COMBAT AIRSPACE — TURN BACK" warning banner and countdown.

### 3. 🎯 Modern Combat Aiming, Hitmarkers & Call of Duty Mobile (CODM) Tactical HUD
- **Authentic Call of Duty Mobile Ergonomics & Layout**:
  - **Left Virtual Thumbstick**: Floating tactical stick with 4 cardinal guide ticks.
  - **Sprint Lock Chevron (`▲ SPRINT`)**: Dragging the thumbstick upward engages automatic afterburner sprint lock. Tapping the chevron toggles lock on/off.
  - **Left-Claw Quick-Fire Trigger**: Dedicated top-left fire trigger for 3-finger or 4-finger claw grip players.
  - **Natural Swipe Touch Aiming Zone**: The entire right 60% of the display acts as a responsive touch-look surface, dynamically adjusting yaw and elevation with sensitivity scaling.
  - **1-Tap ADS Fire Button**: Signature CODM feature—holding this button instantly scopes in (ADS 42° FOV sniper optic) and auto-fires continuous laser bursts while allowing tracking aim. Releasing auto-unscopes.
  - **Dedicated Hip-Fire Button**: Fires tight laser sprays without zooming for wider situational awareness.
  - **Dedicated Scope Toggle Button**: Toggles the sniper optic and holographic reticle on/off.
  - **Fox-2 Homing Missile Button**: Launches heat-seeking missiles with live reloading countdown.
  - **Jump / Climb Thrusters (`▲ CLIMB`) & Slide / Dive Thrusters (`▼ DIVE`)**.
  - **Quick Reset / Respawn Button (`↺ RESET`)**.
  - **Free-Look Eye Button (`👁️`)**: Allows looking 360° around the drone without disrupting the flight path.
  - **Bottom Tactical Weapon Dock**: Dual cards displaying Primary (Pulse Laser) and Secondary (Fox-2 Viper Missiles) with real-time ammunition and recharge status.
  - **Desktop `📱 CODM HUD` Toggle**: Flight OSD bar includes a one-click button to toggle and test the full CODM HUD on desktop and laptops using mouse touch simulation.
- **Pointer-Locked Mouse Aiming & 3D Flight**: Click anywhere on canvas to engage desktop pointer lock; mouse movement directly steers heading (yaw) and elevation (pitch) with smooth aerodynamic bank.
- **ADS Precision Sniper Scope Mode**: Hold Right-Click (or tap mobile `SCOPE` button) to smoothly zoom in from 75° to 42° FOV, displaying a high-contrast holographic optic with digital rangefinder (`RNG: 140M`) and elevation crosshairs.
- **Predictive Lead Indicator Pip**: Real-time HUD trajectory computer calculates moving target lead based on projectile velocity (`time = dist / 165m/s`), displaying a dynamic pulsing lead pip. Aiming at the lead pip guarantees direct hits!
- **Tactical 3D Target Lock-on Box**: Automatically tracks the primary enemy in your crosshair with an authentic CoD lock-on bracket, target ID, rangefinder, and live health bar.
- **Smart Laser Convergence & Anti-Tunneling Raycast**: Dual wing lasers smoothly converge towards the target lead point when inside the aim cone (~36°). Bullet collision uses swept line-segment distance with a generous 6.2m hitbox, eliminating projectile tunneling.
- **Call of Duty Hitmarkers & Audio Feedback**:
  - **White `X` Hitmarker**: Flashes with a sharp, satisfying metallic tick sound on every registered hit.
  - **Floating Damage Numbers**: `24` and `🔥 95 CRIT` numbers erupt in 3D from impacted targets.
  - **Red Skull Kill Confirmation**: `☠️ TARGET DESTROYED +150` banner with heavy bass destruction thud.
- **Continuous Full-Auto Laser Cannon**: Holding Left-Click fires a rapid continuous dual laser stream at ~8.7 rounds/second.
- **Real-Time WebRTC P2P Multiplayer (PeerJS)**:
  - **Invite Link Sharing**: Generate unique room codes (e.g. `SKY-842`) and copy an instant shareable URL (`https://drone-explainer.vercel.app/?room=SKY-842`).
  - **Auto-Join Link Detection**: Friends opening the invite link automatically join the airspace and connect to your flight formation.
  - **3D Remote Drone Synchronization**: High-frequency (~25Hz) smooth position/rotation interpolation, spinning propellers, and synchronized weapon fire.
  - **3D Overhead Nametags & Radar**: Floating illuminated HUD callsign and dynamic health badges (`⚡ Ace-1 [100%]`) and cyan radar blips.
  - **Co-op Swarm & PvP Dogfighting**: Team up against rogue AI drone waves or battle your friends in an intense aerial dogfight with laser and missile hit detection.

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

| Action | Keyboard | Call of Duty Mobile (CODM) Touch Controls |
| :--- | :--- | :--- |
| **Touch Aim & Look** | Mouse (Pointer Lock) / <kbd>Q</kbd> <kbd>E</kbd> | Swipe anywhere on right 60% of screen |
| **Throttle / Strafe** | <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> | Left Tactical Joystick |
| **Auto-Sprint Lock** | <kbd>W</kbd> Afterburner | Drag stick up to `▲ SPRINT` chevron |
| **Left Claw Quick-Fire** | <kbd>F</kbd> | Top-left crosshair trigger (`codm-left-fire`) |
| **1-Tap ADS Auto-Fire** | <kbd>Right-Click</kbd> + <kbd>Left-Click</kbd> | Large circular `ADS FIRE` button (scopes & fires) |
| **Hip-Fire Spray** | <kbd>Left-Click (Hold)</kbd> | Dedicated `HIP` fire button |
| **ADS Sniper Optic** | <kbd>Right-Click (Toggle)</kbd> | Dedicated `SCOPE` toggle button (42° FOV) |
| **Fox-2 Homing Missiles** | <kbd>Middle-Click</kbd> or <kbd>M</kbd> / <kbd>E</kbd> | `FOX-2` button (with live cooldown display) |
| **Ascend / Jump Thrusters** | <kbd>SPACE</kbd> | Tactical `▲ CLIMB` button |
| **Descend / Crouch Thrusters**| <kbd>SHIFT</kbd> | Tactical `▼ DIVE` button |
| **Free-Look (360° Cam)** | Hold <kbd>ALT</kbd> | `👁️` Eye button + swipe |
| **Cycle Camera Mode** | <kbd>C</kbd> | `📹 CAM` button / OSD dropdown |
| **Tactical Weapon Switch** | Keys <kbd>1</kbd> / <kbd>2</kbd> | Tap Primary / Secondary weapon cards |
| **Respawn / Reset** | <kbd>R</kbd> | `↺ RESET` circular button |
| **Toggle Mobile HUD (Desktop)**| — | Top OSD Bar `📱 CODM HUD` button |

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
