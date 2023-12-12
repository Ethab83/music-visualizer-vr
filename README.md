# music-visualizer-vr

customizable music visualizer with vr support

[Click HERE for Demo](https://ethab83.github.io/music-visualizer-vr/)

## Usage

- Upon page load, click play button to start visualization
- Mess around with x and y controls
- Click "Add Modulator" to add a new modulator

### About the modulator

The modulator is inspired by [modular synthesis](https://en.wikipedia.org/wiki/Modular_synthesizer) where you can modulate sound signals using different functions. It has 5 components:

- **Source**: This specifies the source of the data that will be used to modulate the *destination*
- **Destination**: This specifies the object to apply the modulation to.
- **Destination Paramer**: This specifies which parameter of the object should be modulated

## Upcoming features

- Better VR support
- More objects (particles, lights, etc.)
- Ability to add modulator controls as destinations for other modulators.
- Upload your own music
- Use microphone input

## Technology Used

### Audio Parsing

The spectrum analyzer is the brains of the audio parsing. It uses `THREE.AudioAnalyser` to compute a [Fast Fourier Transform](https://en.wikipedia.org/wiki/Fast_Fourier_transform) (mapping amplitude to frequency).

### VR

The VR support is done using [WebXR](https://developer.mozilla.org/en-US/docs/Web/API/WebXR_Device_API). Currently no iPhone support :(

## References

I dont know much css, I just copied the css from three.js examples

- [THREE.js audio visualizer example](https://github.com/mrdoob/three.js/blob/master/examples/webaudio_visualizer.html)
- [THREE.js webgl shaders ocean](https://github.com/mrdoob/three.js/blob/master/examples/webgl_shaders_ocean.html)
- [THREE.js audio visualiser by santosharron](https://github.com/santosharron/audio-visualizer-three-js)
- [simplex-noise.js](https://29a.ch/simplex-noise/docs/index.html#400)
- ChatGPT
- UMass Boston CS460!
