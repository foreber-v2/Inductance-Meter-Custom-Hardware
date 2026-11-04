# Inductance-Meter-Custom-Hardware (Transient Response Method)
Development and modification of an inductance measurement instrument, including schematic redesign, custom PCB layout, fabrication, and experimental testing.

A custom DIY inductance meter built using a CNC-milled PCB, designed to measure inductance directly via transient current pulses and oscilloscope waveform analysis, inspired by classic discrete measurement techniques.

---

## 🛠️ Inspirations & References

This project draws inspiration and conceptual grounding from:
* **[Ludens.cl - LC Meter Design](https://ludens.cl/Electron/lmeter/lmeter.html)** by Ludger Carp: Classic discrete electronic instrumentation and pulse generation.
* **[Hyperspace Pirate - Inductor Tester YouTube Build](https://www.youtube.com/watch?v=IRRF1FadkFw)**: Transistor latch switching and robust pulse-drive stages.

---

## ⚡ Principle of Operation ($V = L \frac{di}{dt}$)

Unlike resonant LC tank meters that calculate inductance based on ringing frequency, this device operates on the fundamental voltage-current relationship of an inductor:

$$V(t) = L \frac{di}{dt}$$

1. **Current Pulse Generation:** The circuit applies a controlled, short-duration current transient through the test inductor.
2. **Waveform Capture:** An oscilloscope captures the resulting voltage and current waveforms across the inductor.
3. **Calculation:** Using the supplied voltage and the rate of change of current ($\frac{di}{dt}$), the inductance ($L$) is derived directly from the transient response curve.

---

## 📸 Process & Hardware Gallery

### 1. Measurement in Progress
<Image src="docs/test/test_in_action.jpg" alt="Inductance meter connected to test setup during measurement" caption="Live measurement in progress on the bench" />

### 2. Device Under Test (DUT)
<Image src="docs/test/inductor_test.jpg" alt="Close-up of the measured inductor component" caption="Sample inductor used for testing" />

### 3. Oscilloscope Waveform Capture
<Image src="docs/waves/wave_2.jpg" alt="Oscilloscope display showing transient voltage and current waveform" caption="Transient voltage and current waveform capture" />

---
