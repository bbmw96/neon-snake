# Neon Snake 2.0

**A revolutionary browser game by [BBMW0 Technologies](https://bbmw0.com)**

Play live: [neon-snake.bbmw0.com](https://neon-snake.bbmw0.com) | [bbmw96.github.io/neon-snake](https://bbmw96.github.io/neon-snake)

---

## What is Neon Snake 2.0?

Neon Snake 2.0 is the most advanced browser snake game ever built. It combines 7 unique biomes, a DNA mutation system, quantum ghost replay, eye tracking via webcam or XR headset, and an adaptive AI opponent with four difficulty levels.

Every game is different. Your mutations carry forward, your ghost chases you next run, and the biome you choose changes both the visuals and the hazards you face.

---

## Features

### 7 Playable Biomes

Each biome has its own colour scheme, grid style, and environmental hazard:

| Biome | Hazard |
|---|---|
| Neon City | None (default) |
| Deep Ocean | Current drift nudges the food |
| The Void | Warp portals teleport the snake |
| Volcano | Lava tiles appear and rotate |
| Forest | Vine walls grow and block paths |
| Arctic | Ice patches cause slide momentum |
| Quantum | Background shimmer and phase distortion |

### DNA Mutation System

Every 8 foods eaten triggers a random genetic mutation. Mutations persist for the rest of the run:

| Mutation | Effect |
|---|---|
| Turbo Gene | Permanent speed increase |
| Twin Food | A second food item spawns |
| Wall Phase | Pass through walls once (adds charges) |
| Echo Ward | Immune to the temporal ghost echo |
| Harvest | Score multiplier on all food |
| Regen | Snake slowly shrinks over time |
| Neural Overload | Doubles the combo window to 6 seconds |

### Quantum Ghost Replay

When you die, your path is saved. On the next game, a purple ghost replays your final moments as a moving obstacle. Outlast your own ghost to unlock the Ghost Slayer achievement.

### Eye Tracking

Steer the snake with your gaze. Two input paths:

- **Webcam** via WebGazer.js (works in any modern browser with camera access)
- **XR headset** via WebXR eye-tracking API (Meta Quest 3/Pro, HTC Vive XR Elite, Ray-Ban Meta)

A consent permission modal appears before any camera or XR session is requested. Your video feed is processed locally and never transmitted.

### Adaptive AI

Four AI modes available from the start screen:

| Mode | Behaviour |
|---|---|
| Off | No AI opponent |
| Easy | BFS pathfinding with random gaps |
| Normal | Full BFS pathfinding |
| Hard | BFS with twin food prioritisation |
| Spectator | Watch the AI play solo |

### Other Mechanics

- **Temporal Echo**: a ghost of your past self from 40 ticks ago replays your path as an obstacle
- **Power-ups**: Speed Boost, Points, Shrink, Shield, Magnet, Slow-Mo
- **Combo system**: eat within the window to multiply your score up to x4
- **Achievements**: 8 unlockable achievements saved to localStorage
- **Procedural audio**: biome-specific sound synthesis via Web Audio API, no external files

---

## Controls

| Input | Action |
|---|---|
| Arrow keys or WASD | Steer |
| Swipe | Steer on mobile |
| Space | Start / restart |
| Eye Track button | Toggle eye tracking |

---

## Technology

| Layer | Implementation |
|---|---|
| Rendering | Canvas 2D API |
| Audio | Web Audio API (synthesised) |
| Eye tracking | WebGazer.js + WebXR Device API |
| State | Vanilla JS, no frameworks |
| Storage | localStorage |
| Deployment | GitHub Pages via GitHub Actions |

---

## Running Locally

No install required. Open the file directly:

```
neon-snake/index.html
```

---

## Deployment

Every push to `main` deploys automatically via GitHub Actions to GitHub Pages.

---

## Credits

Built by [BBMW0 Technologies](https://bbmw0.com). Powered by the BBMW0 Intelligence Engine.

GitHub: [bbmw96/neon-snake](https://github.com/bbmw96/neon-snake)
