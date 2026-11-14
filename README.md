# NIARB // Acoustic Reference Manual & Dual-Node DSP (v6.1)

**NIARB** is an open-source, zero-dependency Web Audio DSP workstation and interactive acoustic manual built with the *Making Software* and *Figma CAD Vector Blueprint* design system.

Standard white, pink, or brown noise masks the human vocal frequency range (300 Hz – 3,000 Hz), forcing the listener's auditory cortex to strain to decode speech consonants and formants. NIARB v6.1 pairs a **Dual-Node Parametric Equalization Architecture** with a dedicated **Master Output Volume Stage** to provide complete acoustic control over lecture study environments.

---

## Technical Architecture & Capabilities

- **Top Master Output Volume Stage:** Dedicated high-precision output fader located directly in the masthead header, featuring click-to-mute toggle and keyboard shortcuts (<kbd>&uarr;</kbd> / <kbd>&darr;</kbd>).
- **Figma CAD Artboard with Dual Rulers:** Hi-DPI 2048-point FFT spectrum framed by precision calibrated top (Hz) and left (dB) technical rulers, with live crosshair cursor telemetry (`CURSOR: -- Hz | -- dB`).
- **Dual-Node Parametric Spline Engine:**
  - **NODE_01 (Left / Blue):** Tunable Biquad Notch filter (600 Hz – 2,200 Hz, $Q = 0.90$) carving out vocal fundamentals and vowel formants.
  - **NODE_02 (Right / Purple):** Tunable Consonant Clarity Peak filter (2,000 Hz – 3,800 Hz, $-4.5\text{ dB}$, $Q = 1.20$) shaping consonant sibilance (*"p", "t", "k", "s"*).
  - **Redline Dimension Indicator:** Dynamic CAD redline vector displaying the frequency interval ($\Delta\text{ Hz}$) between filter vertices.
- **FIG_000 Live Signal Topology Patchbay:** Interactive SVG schematic visualizing signal routing from procedural noise source through cascading filter stages, stereo panning, master gain, and DAC.
- **Blueprint Dark Mode (`[D]`):** Instant toggle between archival warm paper substrate (`#F7F6F2`) and carbon-slate CAD blueprint mode (`#0F1217`).
- **Sticky Margin Index Rail:** Viewport-pinned navigation rail with live parameter telemetry (Master, Notch, Boost, Beat, Theme).
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
| <kbd>&uarr;</kbd> / <kbd>&darr;</kbd> | Adjust Master Output Volume (&plusmn;5%) |
| <kbd>M</kbd> | Toggle Dual-Node Speech Filter (Biquad Notch + Peaking) |
| <kbd>V</kbd> | Toggle Visualizer Mode (FFT Spectrum / Oscilloscope) |
| <kbd>D</kbd> | Toggle CAD Blueprint Dark Mode / Archival Paper Mode |
| <kbd>Click / Drag Canvas</kbd> | Reposition Nearest Active Filter Vertex (Node 01 or Node 02) |
| <kbd>Click "MASTER OUT"</kbd> | Toggle Master Audio Mute |

---

## Usage

Run locally by opening `index.html` or `lecture-focus.html` directly in any modern browser, or deploy to GitHub Pages.
