# Fundamental changelog

### 2.2.2 (in development)
- Mid/Side
	- Normalize decoder mid/side inputs to encoder mid/side outputs.

### 2.2.1 (2022-05-24)
- CV Mix
	- Normalize all inputs to 10V instead of just the first input.

### 2.2.0 (2022-05-22)
- Add CV Mix.
- Add Fade.

### 2.1.0 (2022-01-23)
- VCA Mix
	- When mixing polyphonic and monophonic signals, don't copy monophonic signals to all polyphonic channels. Simply mix them to polyphonic channel 1.
- Scope
	- Change TRIG param options from External/Internal to Disabled/Enabled. External trigger input now requires TRIG param to be enabled.
	- Fix min/max points being read from different buffer phases, creating visual glitches in the waveform plot.

### 2.0.3 (2021-12-31)
- Wavetable VCO and LFO
	- Make wavetable loading lock-free, fixing hiccups and increasing performance.

### 2.0.2 (2021-12-26)
- Wavetable VCO and LFO
	- Fix probabilistic crash when loading wavetable files.

### 2.0.1 (2021-12-18)
- Random
	- Fix rate frequency being 2 times higher than display value.

### 2.0.0 (2021-11-30)
- Mixer
	- When polyphonic and monophonic inputs are combined, copy all mono signals to all mix output poly channels.

### 1.4.1 (2020-07-15)
- Improve VCF model accuracy and stability.

### 1.4.0 (2019-11-08)
- Add Pulses.

### 1.3.1 (2019-10-19)
- Include LEDSliderHandle.svg from Rack v1.1.5 so older versions correctly render panels.

### 1.3.0 (2019-10-19)
- Add Random and Noise modules.
- Make VCA-1 display polyphonic CV.
- Add VU meters to level sliders in Mixer.

### 1.2.1 (2019-08-10)
- Fix VCO hard sync bug, resulting in aliasing.

### 1.2.0 (2019-07-30)
- Add Quantizer.
- Add CV input to Octave.

### 1.1.1 (2019-07-24)
- Mid/Side: fix scaling of decoder.

### 1.1.0 (2019-07-22)
- Add Mid/Side.

### 1.0.1 (2019-06-27)
- Fix VCO-1/2 sync being triggered with a negative slope.

### 1.0.0 (2019-06-19)
- Migrate to v1 API.
- Add performance optimizations with SIMD.
- Change brand to "VCV", so modules appear as "VCV VCO-1", etc.
- Make most modules polyphonic.
- Change VCO-1/2 method from oversampling to MinBLEP.

### 0.5.1 (2017-12-19)
- Added Sequential Switch 1 & 2.

### 0.5.0 (2017-11-21)
- Added 8vert, 8-channel attenuverter.
- Added Unity, 2-channel mixer.
- Changed LED functions in ADSR.

### 0.4.0 (2017-10-13)
- Added Lissajous mode to Scope.
- Added two LFOs and VCO-2.

### 0.3.2 (2017-09-25)
- Fixed Drive CV input of VCF.
- Reverted SEQ3 to continuous gates.
