# Niarb // Acoustic Reference Manual & Dual-Node DSP (v6.0)

**Niarb** is an open-source, zero-dependency Web Audio DSP workstation and interactive acoustic manual built with the *Making Software* and *Figma CAD Vector Blueprint* design system.

Standard white, pink, or brown noise masks the human vocal frequency range (300 Hz – 3,000 Hz), forcing the listener's auditory cortex to strain to decode speech consonants and formants. Niarb v6 introduces a **Dual-Node Parametric Equalization Architecture** that simultaneously carves out the instructor's vocal pitch fundamental while boosting consonant clarity.

---

## Technical Architecture & v6 Capabilities

- **Figma CAD Artboard with Dual Rulers:** Hi-DPI 2048-point FFT spectrum framed by precision calibrated top (Hz) and left (dB) technical rulers, with live crosshair cursor telemetry (`CURSOR: -- Hz | -- dB`).
- **Dual-Node Parametric Spline Engine:**
  - **NODE_01 (Left / Blue):** Tunable Biquad Notch filter (600 Hz – 2,200 Hz, $Q = 0.90$) carving out vocal fundamentals and vowel formants.
  - **NODE_02 (Right / Purple):** Tunable Consonant Clarity Peak filter (2,000 Hz – 3,800 Hz, $+4.5\text{ dB}$, $Q = 1.20$) sharpening consonant sibilance (*"p", "t", "k", "s"*).
  - **Redline Dimension Indicator:** Dynamic CAD redline vector displaying the exact frequency interval ($\Delta\text{ Hz}$) between filter vertices.
- **FIG_000 Live Signal Topology Patchbay:** Interactive SVG schematic visualizing signal routing from procedural noise source through cascading filter stages and stereo panning DAC.
- **Blueprint Dark Mode (`[D]`):** Instant toggle between archival warm paper substrate (`#F7F6F2`) and carbon-slate CAD blueprint mode (`#0F1217`).
- **Sticky Margin Index Rail:** Quick jump navigation and real-time parameter telemetry pinned to the viewport margin.
- **Procedural Noise Engine:** Real-time Brownian (-6 dB/oct), Pink (-3 dB/oct), and White (flat) acoustic masking synthesized directly in browser memory.
- **Anti-Fatigue LFO Modulation (0.12 Hz):** Subtle $\pm 140\text{ Hz}$ sweep preventing cortical habituation over extended study sessions.
- **Neural Phase Entrainment:** Dual-mode Alpha (10 Hz), Beta (18 Hz), and Gamma (40 Hz) entrainment via stereo Binaural beats or speaker-safe Isochronic amplitude pulses.
- **Interactive Reference Manual:** Embedded pedagogical simulators (FIG_002 Formant Collision Simulator with live SNR gain calculation, FIG_003 Animated Phase Vector Engine).
- **Pomodoro Lecture Clock:** 50-minute and 25-minute study intervals with automatic noise floor ducking and a synthesized 528 Hz / 880 Hz harmonic chime.

---

## Keyboard Shortcuts

| Key | Action |
| :--- | :--- |
| <kbd>Space</kbd> | Engage / Disengage Audio Engine |
| <kbd>M</kbd> | Toggle Dual-Node Speech Filter (Biquad Notch + Peaking) |
| <kbd>V</kbd> | Toggle Visualizer Mode (FFT Spectrum / Oscilloscope) |
| <kbd>D</kbd> | Toggle CAD Blueprint Dark Mode / Archival Paper Mode |
| <kbd>Click / Drag Canvas</kbd> | Reposition Nearest Active Filter Vertex (Node 01 or Node 02) |

---

## Usage

Run locally by opening `index.html` or `lecture-focus.html` directly in any modern browser, or deploy to GitHub Pages.
