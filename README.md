# Orrery — Solar System Simulation

An accelerated, real-date simulation of the solar system in the browser. Built with [three.js](https://threejs.org), no build step.

**Live:** https://daniel-burla.github.io/solar-system/

## What it does

- Planet positions come from JPL's Keplerian elements (J2000 with secular rates), solved each frame, so the sky matches the real date. Press **N** to jump to now.
- Adjustable time rate from real time up to ~3 years per second, forward or reverse.
- Sun, eight planets, seven major moons (Moon, Io, Europa, Ganymede, Callisto, Titan, Triton), Saturn and Uranus rings, axial tilts and real rotation periods, Earth night lights and clouds.
- Compressed scale by default so everything stays visible; a **True scale** toggle shows real distances and sizes.
- Procedural starfield plus a Milky Way sky, bloom on the Sun, glass-panel HUD.

## Controls

| Key | Action |
| --- | --- |
| Space | Play / pause |
| , . | Slower / faster |
| R | Reverse time |
| N | Jump to now |
| 0–8 | Sun, Mercury … Neptune |
| Esc | Back to overview |
| O / L / T / G | Orbits / Labels / True scale / Glow |
| H | Hide HUD |

Click any body or label to follow it. Drag to orbit, scroll to zoom.

## Run locally

Any static server works, for example:

```bash
python3 -m http.server 5173
```

## Credits

- Planet, Moon, ring and sky textures: [Solar System Scope](https://www.solarsystemscope.com/textures/), CC BY 4.0.
- Orbital elements: JPL Solar System Dynamics, *Keplerian Elements for Approximate Positions of the Major Planets*.
- Physical data: NASA planetary fact sheets.
