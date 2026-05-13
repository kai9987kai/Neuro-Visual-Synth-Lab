# Neuro-Visual Synth Lab

**Neuro-Visual Synth Lab** is a single-file browser experiment for generative audio, procedural visuals, creative challenges, and lightweight self-observation. It combines Web Audio synthesis, canvas-based visual systems, reaction-diffusion simulation, boids, neural-style flow fields, adaptive session tools, and a creative challenge generator in one portable HTML file.

> ⚠️ **Important safety note:** This project is an experimental creative tool, not a medical, therapeutic, diagnostic, or cognitive-enhancement device. Keep volume low, stop immediately if you feel discomfort, and avoid intense flashing visuals if you have photosensitivity, epilepsy risk, migraine sensitivity, dizziness, anxiety, or sensory sensitivity.

---

## ✨ Highlights

- **Single-file app** — runs as one standalone `.html` file.
- **Generative audio engine** with binaural-style frequency difference controls, carrier frequency, noise texture, pulse modulation, stereo width, waveform selection, drift, smoothing, breath envelope, and limiter.
- **Multiple visual engines**
  - Plasma field
  - Boids / flocking
  - Reaction-diffusion
  - Neural flow field
  - Audio scope ring
  - Chaotic attractors
  - Synaptic map
- **Audio-reactive visuals** that respond to the audio engine and session state.
- **Safety-aware controls**
  - Flash-safe visual guard
  - Brightness limiting
  - Reduced-motion option
  - Panic stop
  - Conservative default volume
  - Session timer
- **Creative challenge generator** with random seeds, difficulty levels, practical constraints, and project ideas tuned for web labs, procedural sims, 3D, audio, Unity, AI/ML thinking, and 3D printing.
- **Lab protocol tools** for structured mini-experiments.
- **Session journal** with before/after ratings, notes, saved local history, and CSV export.
- **Preset system** with save/load/import/export.
- **PNG export** for visual snapshots.
- **No backend required** — all computation happens locally in the browser.

---

## 🎛️ What It Does

Neuro-Visual Synth Lab is designed as a creative sandbox for exploring the relationship between:

- sound design,
- procedural animation,
- emergent systems,
- attention-state journaling,
- audio-reactive art,
- challenge-based learning,
- and experimental interface design.

It does **not** claim to entrain brainwaves, improve cognition, treat anxiety, treat sleep issues, or provide clinical benefits. Binaural beats, isochronic pulse patterns, and rhythmic audio can feel interesting, but effects vary strongly by person and context. This app keeps those controls transparent and user-adjustable rather than hiding them behind medical-style claims.

---

## 🚀 Quick Start

### Option 1: Open directly

1. Download or clone the project.
2. Open the HTML file in a modern browser.
3. Click **Start Audio Engine** if you want sound.
4. Use the tabs to explore audio, visuals, lab tools, challenges, and journaling.

### Option 2: Run with a local server

Some browsers behave more consistently with local files when served through `localhost`.

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

---

## 🧩 Main Tabs

### Audio

Controls the Web Audio engine.

Common controls include:

- **Master Volume** — overall output level.
- **Carrier Frequency** — base tone frequency.
- **Binaural Beat Δ** — difference between left and right oscillator frequencies.
- **Noise Mix** — shaped noise texture.
- **Isochronic Pulse** — amplitude pulse rate.
- **Stereo Width** — spread between left and right channels.
- **Waveform** — oscillator shape.
- **Noise Type** — white, pink, or brown-style noise.
- **Micro Drift** — subtle modulation for less static tones.
- **Beat Smoothing** — reduces abrupt frequency changes.
- **Breath Envelope** — slow amplitude shaping for gentler sessions.
- **Quick Presets** — starting points such as focus-ish, chill, and deep.

The audio system uses ramping and a dynamics compressor/limiter to reduce harsh transitions and clipping risk.

---

### Visual

Controls the procedural canvas renderer.

Visual modes include:

| Mode | Description |
|---|---|
| Plasma | Fast shader-like color field rendered on canvas |
| Boids | Emergent flocking particles using separation, alignment, and cohesion |
| Reaction-Diffusion | Gray-Scott style organic pattern system |
| Neural Flow Field | Particle-like motion guided by procedural vector fields |
| Audio Scope Ring | Circular waveform/ring visualization |
| Chaotic Attractors | Dynamical-system-inspired motion trails |
| Synaptic Map | Node-and-edge visual field with pulsing connection behavior |

Visual controls include:

- **Visual Speed**
- **Intensity**
- **Brightness Cap**
- **Boids Count**
- **Reaction-Diffusion Iterations**
- **Feed / Kill parameters**
- **Flash-Safe Guard**
- **Reduced Motion**
- **Audio-Reactive Coupling**
- **Randomize Visuals**
- **Export PNG**

---

### Challenge

Generates random creative and technical micro-challenges.

Example challenge categories:

- Web dev
- Procedural simulation
- 3D modeling
- 3D printing
- Unity audio
- Creative prompt design
- AI/ML thinking
- Systems benchmarking
- Interface design
- Research prototyping

Each challenge can include:

- a seed,
- a domain,
- constraints,
- difficulty,
- a twist,
- and practical deliverables.

---

### Lab

Provides a more structured experimental workflow.

Useful for running small sessions like:

1. Choose one variable to change.
2. Keep the volume low.
3. Run a short timed session.
4. Write before/after ratings.
5. Save notes.
6. Export results as CSV.

This is meant for personal observation and creative process tracking, not clinical measurement.

---

### Journal

The journal lets you record:

- before-session rating,
- after-session rating,
- notes,
- selected mode,
- audio settings,
- visual settings,
- timestamp,
- session duration.

Data is stored locally in the browser using `localStorage`. You can export a CSV for analysis in spreadsheet tools.

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|---|---|
| `Space` | Toggle audio engine |
| `V` | Cycle visual modes |
| `Esc` | Panic stop / stop audio and reduce stimulation, if implemented |
| Mouse click | Inject reaction-diffusion disturbance or interact with visuals |
| Mouse drag | Repel/attract boids or inject continuous disturbances depending on mode |

---

## 🖼️ Visual Interaction

- Click the canvas in **Reaction-Diffusion** mode to inject an “ink drop.”
- Hold or drag the pointer to continuously disturb the simulation.
- In **Boids** mode, pointer movement influences flock behaviour.
- In audio-reactive modes, visual motion and shape respond to audio parameters and RMS-like internal signal estimates.

---

## 🔊 Audio Design Notes

The audio system is intentionally transparent and conservative.

It includes:

- oscillators for left/right tones,
- optional binaural-style frequency difference,
- shaped noise,
- pulse modulation,
- stereo width control,
- limiter/compressor,
- parameter ramping,
- low default volume,
- stop button,
- panic-style safety behaviour,
- and session timing.

Recommended usage:

- Use headphones only at a low, comfortable level.
- Start with low volume.
- Avoid long sessions.
- Change one parameter at a time.
- Stop if you feel discomfort, headache, dizziness, agitation, nausea, ear pressure, or visual strain.

---

## ⚠️ Safety Guidance

Do **not** use this tool while driving, operating equipment, or doing anything that requires full attention.

Avoid or use extra caution if you have:

- epilepsy or seizure history,
- photosensitive epilepsy risk,
- migraine sensitivity,
- vestibular issues,
- tinnitus or hearing sensitivity,
- panic/anxiety sensitivity,
- neurological conditions,
- recent head injury,
- severe sleep deprivation,
- or discomfort with rhythmic audio/visual stimulation.

The app includes a flash-safe guard and brightness controls, but no software guard can guarantee safety for every person, device, display, refresh rate, or environment.

---

## 🧠 Research-Informed Direction

The design follows a cautious experimental approach:

- **Binaural and rhythmic audio effects are treated as exploratory**, not guaranteed.
- **User control matters**: volume, frequency, pulse, drift, width, noise, and session length are adjustable.
- **Smooth transitions are preferred** to abrupt jumps.
- **Visual intensity needs guardrails**, especially for flashing, brightness, and high-speed motion.
- **Self-tracking should be lightweight** and should avoid medical interpretation.
- **Creative challenge systems can encourage learning** by adding constraints, randomness, and reflection.

The project is best understood as a creative coding lab that borrows ideas from sound design, generative art, human-computer interaction, and self-experiment journaling.

---

## 🏗️ Technical Architecture

The app is built using standard browser APIs:

- **HTML** for structure
- **CSS** for responsive glass-panel UI
- **Canvas 2D** for visual rendering
- **Web Audio API** for synthesis and signal routing
- **localStorage** for presets and journal history
- **Blob downloads** for PNG/CSV/export files
- **Vanilla JavaScript** for all logic

No build step is required.

---

## 🧪 Core Systems

### 1. Audio Engine

Main nodes:

- `AudioContext`
- `OscillatorNode`
- `GainNode`
- `ChannelMergerNode`
- `BiquadFilterNode`
- `BufferSourceNode`
- `ConstantSourceNode`
- `DynamicsCompressorNode`

The engine supports:

- left/right oscillator offset,
- shaped noise buffer generation,
- amplitude pulse modulation,
- master gain ramping,
- limiter/compression,
- and safe start/stop behaviour.

---

### 2. Plasma Renderer

A reduced-resolution canvas image buffer is generated and scaled up for a pixelated fast visual effect.

Features:

- sine/cosine field interference,
- mouse influence,
- spectral-style color mapping,
- speed/intensity controls.

---

### 3. Boids Renderer

Implements classic flocking behaviour:

- separation,
- alignment,
- cohesion,
- pointer influence,
- screen wrapping,
- simple spatial hash optimization,
- trails and glow rendering.

---

### 4. Reaction-Diffusion

Uses a Gray-Scott style simulation with:

- A/B chemical fields,
- feed/kill controls,
- diffusion,
- laplacian sampling,
- pointer injection,
- adjustable iterations per frame.

This produces organic spots, waves, coral-like structures, cellular fields, and unstable pattern transitions.

---

### 5. Neural Flow Field

A procedural vector-field mode that gives a neural-map / signal-path aesthetic.

Possible behaviours:

- seeded particles,
- directional drift,
- field turbulence,
- audio-reactive acceleration,
- glow trails,
- pointer influence.

---

### 6. Audio Scope Ring

A visual oscilloscope-style mode rendered as a radial ring.

Possible behaviours:

- pulse-reactive radius,
- frequency-driven deformation,
- volume-driven glow,
- stereo/beat-influenced wobble.

---

### 7. Chaotic Attractors

A dynamical-system-inspired visual mode.

Possible behaviours:

- attractor traces,
- rotating phase fields,
- decay trails,
- high-density glowing paths,
- audio-reactive parameter changes.

---

### 8. Synaptic Map

A node graph visualization inspired by neural connection maps.

Possible behaviours:

- pulsing nodes,
- weighted links,
- local clusters,
- moving activation waves,
- pointer-induced excitation,
- audio-reactive connection strength.

---

## 💾 Presets and Storage

The app can save local presets using browser storage.

Preset data may include:

- audio parameters,
- visual parameters,
- lab settings,
- safety settings,
- selected mode,
- and UI preferences.

Because storage is local:

- presets stay in the same browser/profile,
- clearing browser data may delete them,
- no data is uploaded anywhere.

---

## 📤 Export Features

Depending on the current version, export tools may include:

- **PNG snapshot** of the visual canvas
- **CSV journal export**
- **Preset JSON export**
- **Preset JSON import**
- **Challenge copy**
- **Protocol copy**

---

## 📁 Suggested File Structure

For a single-file version:

```text
neuro-visual-synth-lab/
├── index.html
├── README.md
└── LICENSE
```

For a future expanded version:

```text
neuro-visual-synth-lab/
├── index.html
├── README.md
├── LICENSE
├── assets/
│   └── screenshots/
├── docs/
│   ├── safety.md
│   ├── research-notes.md
│   └── experiments.md
└── examples/
    └── presets/
```

---

## 🧭 Suggested Workflow

A safe creative workflow:

1. Open the app.
2. Keep volume low.
3. Start with visuals only.
4. Enable audio only when ready.
5. Pick one visual mode.
6. Change one parameter at a time.
7. Run short sessions.
8. Use the journal tab to record observations.
9. Export snapshots or CSV if you want to compare sessions.

---

## 🛠️ Development Ideas

Possible next upgrades:

- WebGL shader renderer for faster plasma and flow fields
- WebGPU compute version of reaction-diffusion
- MIDI controller input
- Microphone input for external audio-reactive visuals
- Timeline sequencer for parameter automation
- Visual preset gallery
- Built-in screenshot gallery
- Audio recording/export
- Offline PWA support
- Session replay
- More advanced accessibility settings
- Colorblind-safe palettes
- WebXR immersive visual mode
- Multi-canvas compositor
- Worker-based simulation thread
- GLSL reaction-diffusion
- Real FFT analyser view
- Modular patch graph for audio + visuals
- “Research protocol builder” with randomized A/B conditions

---

## 🧑‍💻 Browser Support

Recommended:

- Chrome / Chromium
- Edge
- Firefox
- Safari with modern Web Audio support

For best results:

- use a desktop browser,
- enable hardware acceleration,
- avoid battery saver mode,
- use headphones carefully and quietly if testing stereo audio.

---

## 🐛 Troubleshooting

### Audio does not start

Browsers require a user gesture before audio can begin. Click the **Start Audio Engine** button.

### Audio is too loud or harsh

Lower master volume immediately or press stop. Keep headphones at low volume.

### Visuals are slow

Try:

- reducing boid count,
- lowering reaction-diffusion iterations,
- turning on reduced motion,
- using plasma mode,
- closing other tabs,
- lowering browser zoom or display scale.

### Presets disappeared

Browser localStorage may have been cleared.

### The canvas looks blurry

The app balances performance and resolution. Some modes intentionally render at reduced resolution and scale up.

---

## 🤝 Contributing

Ideas, improvements, and experiments are welcome.

Good contribution areas:

- safer defaults,
- better accessibility,
- more visual modes,
- performance optimization,
- WebGL/WebGPU renderers,
- better preset management,
- more challenge templates,
- stronger documentation,
- mobile UI improvements,
- better session export tools.

When contributing, avoid adding medical claims unless they are carefully sourced, limited, and clearly framed as non-clinical.

---

## 📜 License

Recommended license: **MIT**.

Add a `LICENSE` file if publishing publicly.

---

## Disclaimer

This project is for creative coding, generative art, sound design, and personal experimentation only.

It is not medical software. It does not diagnose, treat, prevent, or cure any condition. Audio and visual stimulation can be uncomfortable or risky for some people. Use responsibly, keep intensity low, and stop immediately if you feel unwell.
