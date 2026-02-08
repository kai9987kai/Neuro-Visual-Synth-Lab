# Neuro-Visual-Synth-Lab

**Neuro-Visual-Synth-Lab** is a **single-file, in-browser lab** that combines a **live audio engine** (binaural / isochronic / noise) with multiple **real-time visual modes** (Plasma / Boids / Reaction-Diffusion) plus a **random challenge generator** for guided experiments. :contentReference[oaicite:0]{index=0}

This repo is intentionally minimal: it currently ships as a single `index.html` you can open locally or host via GitHub Pages. :contentReference[oaicite:1]{index=1}

---

## What’s included

### Audio (Web Audio API)
- **Binaural beats**: dual tones (L/R) with a small frequency offset to create a perceived beat frequency.
- **Isochronic pulses**: a carrier tone gated (hard/soft) by an LFO/pulse train to create distinct rhythmic “on/off” stimulation.
- **Noise generator**: white/pink-ish style noise (implementation-dependent), often paired with filters for texture.
- Typical signal chain concepts you’ll see in this kind of build:
  - `OscillatorNode` / noise buffer → shaping (gain/LFO) → optional filtering → master gain → destination
- Browser note: audio playback generally requires a **user gesture** (click/tap) to start/resume the `AudioContext`.

(Repo description explicitly states binaural/isochronic/noise as the core audio engine.) :contentReference[oaicite:2]{index=2}

### Visuals (Canvas)
- **Plasma**: procedural field / shader-style color motion (often sin/cos fields, turbulence, or noise-based warps).
- **Boids**: flocking simulation (separation / alignment / cohesion) rendered as particles or glyphs.
- **Reaction-Diffusion**: Gray-Scott-style pattern formation (feed/kill parameters evolving textures over time).

(Repo description explicitly lists Plasma / Boids / Reaction-Diffusion as visual modes.) :contentReference[oaicite:3]{index=3}

### Random Challenge Generator
A lightweight “prompt engine” to suggest experiments, e.g.:
- “Pick a beat frequency, then tune reaction-diffusion until you get stable spots.”
- “Switch to Boids and increase density while keeping audio comfortable.”
- “Try noise + filter sweep and see which visual mode feels most ‘locked in’.”

(Repo description explicitly lists a random challenge generator.) :contentReference[oaicite:4]{index=4}

---

## Quick start

### Option A — Run locally (double-click)
1. Download / clone the repo
2. Open `index.html` in a modern browser (Chrome/Edge/Firefox).

If your browser blocks certain features under `file://`, use Option B.

### Option B — Run via a tiny local server (recommended)
From the repo directory:

**Python**
```bash
python -m http.server 8000
