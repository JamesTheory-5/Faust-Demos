# Faust-Demos

Absolutely! 🎛️
Here’s a **comprehensive guide** to the **Faust Examples and Demos** — from the official Faust ecosystem and practical categories you can explore, experiment with, and modify.

---

# 🎵 **Faust Examples and Demos Overview**

The Faust ecosystem comes with an extensive set of **example programs**, grouped by category, demonstrating everything from **basic DSP blocks** to **complete synthesizers**, **effects**, and **interactive systems**.

You can access them directly from:

* [📚 Faust Libraries & Examples](https://faustdoc.grame.fr)
* [🎹 Faust IDE / Playground](https://faustide.grame.fr)
* `examples/` directory in the Faust source tree or FaustLive app.

---

## 🎧 1. **Basic DSP Building Blocks**

These examples teach you the foundation of Faust’s functional DSP language.

| Example          | Description                                                                   |
| ---------------- | ----------------------------------------------------------------------------- |
| `oscillator.dsp` | Sine, square, saw, triangle wave generators using `os.osc`, `os.square`, etc. |
| `noise.dsp`      | White, pink, brown noise generators (`no.noise`, `no.pink_noise`).            |
| `filters.dsp`    | Lowpass, highpass, bandpass filters using `fi.lowpass`, `fi.highpass`, etc.   |
| `adsr.dsp`       | ADSR envelope generator (attack, decay, sustain, release).                    |
| `gain.dsp`       | Simple gain control (`*(slider("gain",1,0,2,0.01))`).                         |
| `pan.dsp`        | Stereo panning demo using `ba.pan2`.                                          |

🧠 *Learn core Faust syntax: function definitions, block-diagram composition (`:`, `,`, `~`), and recursion.*

---

## 🎸 2. **Synthesizers**

| Example              | Description                                                                 |
| -------------------- | --------------------------------------------------------------------------- |
| `karplusstrong.dsp`  | Plucked string synthesis using Karplus–Strong algorithm.                    |
| `fm.dsp`             | FM synthesis demo with carrier and modulator frequency sliders.             |
| `sawSynth.dsp`       | Basic subtractive synth with sawtooth oscillator + filter + envelope.       |
| `organ.dsp`          | Additive organ synthesis with harmonics and amplitude envelopes.            |
| `polyphonic.dsp`     | Demonstrates MIDI-driven polyphony via `midi.poly`.                         |
| `physical_modeling/` | Contains instruments like flute, clarinet, membrane, and string resonators. |

🎧 *Run in FaustLive or Playground with MIDI input for instant synth demos.*

---

## 🎚️ 3. **Audio Effects**

| Category         | Examples                                          | Description                                          |
| ---------------- | ------------------------------------------------- | ---------------------------------------------------- |
| **Reverb**       | `reverb.dsp`, `freeverb.dsp`, `zita_rev1.dsp`     | Room/plate reverbs based on `rev.*` and `zita_rev1`. |
| **Delay**        | `delay.dsp`, `pingpong_delay.dsp`                 | Simple and stereo ping-pong delays.                  |
| **Compressor**   | `compressor.dsp`, `abs_envelope_t60.dsp`          | Dynamic range compression with envelope tracking.    |
| **Distortion**   | `distortion.dsp`, `overdrive.dsp`, `fuzz.dsp`     | Analog-style saturation and waveshaping.             |
| **EQ / Filter**  | `equalizer.dsp`, `tone_control.dsp`, `wahwah.dsp` | Parametric EQ and dynamic filtering.                 |
| **Pitch / Time** | `pitch_shift.dsp`, `chorus.dsp`, `flanger.dsp`    | Modulation and delay-based FX.                       |

🎛️ *Each effect demonstrates different DSP libraries: `filters.lib`, `envelopes.lib`, `compressors.lib`, etc.*

---

## 🎤 4. **Dynamic Processing & Utilities**

| Example                 | Description                                      |
| ----------------------- | ------------------------------------------------ |
| `compressor_simple.dsp` | Classic feed-forward compressor.                 |
| `gate.dsp`              | Noise gate with threshold and hold time.         |
| `limiter.dsp`           | Brick-wall limiter using fast envelope follower. |
| `metering.dsp`          | RMS and peak level meters.                       |
| `envelope_follow.dsp`   | Shows use of `abs_envelope_t60`.                 |

🧩 *These examples are great to combine with others for building DAW-style plugins.*

---

## 🎛️ 5. **Control and Interaction**

| Example                | Description                                                       |
| ---------------------- | ----------------------------------------------------------------- |
| `ui_demo.dsp`          | Shows how to create Faust GUIs using sliders, knobs, and buttons. |
| `midi.dsp`             | Receives MIDI messages and maps them to parameters.               |
| `osc_demo.dsp`         | Control Faust parameters over OSC (Open Sound Control).           |
| `touchosc_example.dsp` | Example for mobile/tablet control.                                |

📡 *Explore how Faust interacts with external controllers and sensors.*

---

## 🎮 6. **Advanced / Interactive Examples**

| Example                         | Description                                            |
| ------------------------------- | ------------------------------------------------------ |
| `physical_modeling/guitar.dsp`  | Realistic plucked string synthesis.                    |
| `physical_modeling/violin.dsp`  | Bowed-string model using nonlinear interaction.        |
| `spatialization/ambisonic.dsp`  | 3D audio and surround sound encoding.                  |
| `machine_learning/faust2nn.dsp` | Using neural-network-based controllers.                |
| `faust2api` examples            | Shows integration with C++, JUCE, or PureData targets. |

🧠 *Showcases Faust’s power for academic and experimental DSP research.*

---

## 🎧 7. **Complete Demos (Ready to Play)**

You can load these in [Faust IDE](https://faustide.grame.fr) or compile them for your DAW or hardware:

| Demo                  | What It Does                                            |
| --------------------- | ------------------------------------------------------- |
| `freeverb_demo.dsp`   | Reverb effect chain with adjustable parameters.         |
| `synth_demo.dsp`      | Polyphonic synth playable via MIDI.                     |
| `compressor_demo.dsp` | Stereo compressor with visual meter.                    |
| `pedalboard_demo.dsp` | Guitar FX chain (distortion → chorus → delay → reverb). |
| `drum_machine.dsp`    | Simple trigger-based drum generator.                    |

---

## 🧠 Learning Tip

If you’re exploring:

* Start in [**Faust Playground**](https://faustplayground.grame.fr)
  → Try examples live in your browser.
* Then explore:
  **`examples/` folder** inside Faust → subfolders:

  ```
  basics/
  effects/
  instruments/
  filters/
  physical_modeling/
  synths/
  ...
  ```

---

Would you like me to give you a **list of recommended demo chains** (e.g., "Build a simple synth → add delay → add reverb") or **ready-to-copy code templates** for a few *showcase-level examples* (like a “mini DAW chain” or “poly synth with FX”)?

---

You can drop this as a prompt to start.
