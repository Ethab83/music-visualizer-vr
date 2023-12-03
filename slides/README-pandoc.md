---
title: music-visualizer-vr
author: Ethan Mulcahy
date: \today
output: beamer_presentation
institute: University of Massachusetts, Boston
theme: metropolis
---

## Usage

[Click HERE for Demo](https://ethab83.github.io/music-visualizer-vr/)

- Upon page load, click play button to start visualization
- Mess around with x and y controls
- Click "Add Modulator" to add a new modulator
    - no actual functionality yet

---

## About the modulator

The modulator is inspired by [modular synthesis](https://en.wikipedia.org/wiki/Modular_synthesizer) where you can modulate sound signals using different functions. It has 5 components:

- **Source**: This specifies the source of the data that will be used to modulate the *destination*
- **Destination**: This specifies the object to apply the modulation to.
- **Destination Paramer**: This specifies which parameter of the object should be modulated

---

## About the Spectrum Analyzer

The spectrum analyzer is the brains of the audio parsing. It uses `THREE.AudioAnalyser` to compute a Fast Fourier Transform (mapping amplitude to frequency) for every call to the animation loop.

The frequency ranges (e.g. Bass, Treble, Volume) are then calculated by averaging the amplitude values in a set range.

---

## Upcoming features

- Ability to add moculator x and y controls as destinations.
- Separate modulator into 3D and 2D modulators
- More objects?

---

## References

- [THREE.js audio visualizer example](https://github.com/mrdoob/three.js/blob/master/examples/webaudio_visualizer.html)
- [THREE.js audio visualiser by santosharron](https://github.com/santosharron/audio-visualizer-three-js)
- ChatGPT
- UMass Boston CS460!
