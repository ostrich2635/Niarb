# Niarb

**Niarb** is a zero-dependency Web Audio DSP synthesizer designed for students and engineers listening to lectures. Standard white, pink, or brown noise masks the human vocal frequency range (300 Hz – 3,000 Hz), making instructors harder to understand. Niarb uses a real-time tunable band-reject notch filter to carve out the lecturer's vocal fundamental and formant frequencies while masking surrounding environmental distractions.

## Core Capabilities

- **Tunable Vocal-Notch Carve (600 Hz – 2500 Hz):** Interactive Biquad band-reject filter with a 0.12 Hz anti-fatigue LFO sweep. Click or drag directly on the FFT spectrum canvas to tune the notch center.
- **Procedural Noise Engine:** Real-time Brownian, Pink ($1/f$), and White noise synthesis in browser memory.
- **Binaural & Isochronic Neural Entrainment:** Supports stereo Binaural Beats (Alpha 10 Hz, Beta 18 Hz, Gamma 40 Hz) for headphones and amplitude-modulated Isochronic Pulses for laptop speakers.
- **140Hz Hi-DPI Spectrum & Oscilloscope:** 2048-point FFT analyzer with visual speech-notch reticle.
- **Pomodoro Lecture Timer:** 50-minute and 25-minute focus blocks with automatic noise floor ducking and a synthesized 528 Hz / 880 Hz harmonic bell chime.

## Usage

Open `index.html` or `lecture-focus.html` directly in any modern browser.
