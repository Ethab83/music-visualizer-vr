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

- Upon page load, click ![play button](play_button.png){width=40} to start visualization
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

## Upcoming features

- Better VR support
- More objects (particles, lights, etc.)
- Ability to add modulator controls as destinations for other modulators.
- Upload your own music
- Use microphone input

---

## Technology Used

### Audio Parsing

The spectrum analyzer is the brains of the audio parsing. It uses `THREE.AudioAnalyser` to compute a [Fast Fourier Transform](https://en.wikipedia.org/wiki/Fast_Fourier_transform) (mapping amplitude to frequency).

### VR

The VR support is done using [WebXR](https://developer.mozilla.org/en-US/docs/Web/API/WebXR_Device_API). Currently no iPhone support :(

---

## References

- [THREE.js audio visualizer example](https://github.com/mrdoob/three.js/blob/master/examples/webaudio_visualizer.html)
- [THREE.js audio visualiser by santosharron](https://github.com/santosharron/audio-visualizer-three-js)
- ChatGPT
- UMass Boston CS460!
