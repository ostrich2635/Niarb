# Niarb // Acoustic Reference Manual & Lecture DSP (v5.0)

**Niarb** is an open-source, zero-dependency Web Audio DSP workstation and interactive acoustic manual designed in the *Making Software* and *Figma Vector Blueprint* editorial aesthetic.

Standard white, pink, or brown noise masks the human vocal frequency range (300 Hz – 3,000 Hz), forcing the brain's auditory cortex to strain to decode speech consonants and formants. Niarb uses a real-time tunable Biquad band-reject notch filter to carve out the instructor's vocal formant band while masking ambient environmental noise.

---

## Technical Features

- **FIG_001 Real-Time 2048-pt FFT Spectrum & Bézier Notch Node:** Interactive canvas with Figma vector coordinates, tangent handles, and direct click/drag frequency tuning (600 Hz – 2,500 Hz).
- **Procedural Noise Engine:** Real-time Brownian (-6 dB/oct), Pink (-3 dB/oct), and White (flat) acoustic masking synthesized directly in browser memory.
- **Anti-Fatigue LFO Modulation (0.12 Hz):** Subtle ±140 Hz oscillator drift that prevents auditory habituation over long study blocks.
- **Neural Phase Entrainment (Binaural & Isochronic):**
  - **Binaural Beats:** Dual-channel phase interference (Alpha 10 Hz, Beta 18 Hz, Gamma 40 Hz) over a tunable fundamental carrier (140 Hz – 320 Hz) for headphones.
  - **Isochronic Pulse Mode:** Amplitude-modulated pulses for laptop and external stereo speakers without phase cancellation.
- **FIG_002 Speech Formant Collision Simulator:** Interactive pedagogical simulator demonstrating Signal-to-Noise Ratio (SNR) clarity improvements when carving acoustic space for human speech.
- **FIG_003 Animated Phase Math Engine:** Real-time SVG vector rendering of carrier wave interference envelopes versus amplitude-rectified pulses.
- **Pomodoro Lecture Clock:** 50-minute and 25-minute focus intervals featuring automatic noise floor ducking (25%) and a synthesized 528 Hz / 880 Hz harmonic chime.
- **Hardware Presets & Local State:** One-click presets for Male Lecturers (850 Hz), Female Lecturers (1650 Hz), STEM Problem Sets (1200 Hz Beta), and Deep Cramming (Pink Gamma), persisted via `localStorage`.

---

## Keyboard Shortcuts

| Key | Action |
| :--- | :--- |
| <kbd>Space</kbd> | Engage / Disengage Audio Engine |
| <kbd>M</kbd> | Toggle Speech Band Carve Filter (Biquad Notch) |
| <kbd>V</kbd> | Toggle Visualizer Mode (FFT Spectrum / Oscilloscope) |
| <kbd>Click / Drag Canvas</kbd> | Reposition Vocal Notch Center Frequency ($f_0$) |

---

## Usage

Run locally by opening `index.html` or `lecture-focus.html` in any modern web browser, or view live on GitHub Pages.
