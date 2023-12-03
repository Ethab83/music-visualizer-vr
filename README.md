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

- Ability to add moculator x and y controls as destinations.
- Separate modulator into 3D and 2D modulators

## About the Spectrum Analyzer

The spectrum analyzer is the brains of the audio parsing. It uses `THREE.AudioAnalyser` to compute a Fast Fourier Transform (mapping amplitude to frequency) for every call to the animation loop.

The frequency ranges (e.g. Bass, Treble, Volume) are then calculated by averaging the amplitude values in a set range.

## References

I dont know much css, I just copied the css from three.js examples

- [THREE.js audio visualizer example](https://github.com/mrdoob/three.js/blob/master/examples/webaudio_visualizer.html)
- [THREE.js audio visualiser by santosharron](https://github.com/santosharron/audio-visualizer-three-js)
- ChatGPT
- UMass Boston CS460!
