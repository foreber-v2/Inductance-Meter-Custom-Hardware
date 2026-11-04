# Inductance-Meter-Custom-Hardware (Transient Response Method)
Development and modification of an inductance measurement instrument, including schematic redesign, custom PCB layout, fabrication, and experimental testing.

A custom DIY inductance meter built using a CNC-milled PCB, designed to measure inductance directly via transient current pulses and oscilloscope waveform analysis, inspired by classic discrete measurement techniques.

---

## 🛠️ Inspirations & References

This project is built upon foundational concepts and schematics adapted from classic discrete designs. The hardware merges elements from both sources, customized and optimized with original modifications:
* **[Ludens.cl - Power inductor tester](https://ludens.cl/Electron/lmeter/lmeter.html)** 
* **[Hyperspace Pirate - Inductor Tester YouTube Build](https://www.youtube.com/watch?v=IRRF1FadkFw)**

---

## ⚡ Principle of Operation ($V = L \frac{di}{dt}$)

Unlike resonant LC tank meters that calculate inductance based on ringing frequency, this device operates on the fundamental voltage-current relationship of an inductor:

$$V(t) = L \frac{di}{dt}$$

1. **Current Pulse Generation:** The circuit applies a controlled, short-duration current transient through the test inductor.
2. **Waveform Capture:** An oscilloscope captures the resulting voltage and current waveforms across the inductor.
3. **Calculation:** Using the supplied voltage and the rate of change of current ($\frac{di}{dt}$), the inductance ($L$) is derived directly from the transient response curve.

---
## 📂 kicad and firmaware files Coming Soon!!!

## 📸 Process & Hardware Gallery

### 1. Measurement in Progress
<a href="images/measurement_setup.jpg" target="_blank">
  <img src="images/measurement_setup.jpg" alt="Live measurement in progress on the bench" width="300px" />
</a>

### 2. Device Under Test (DUT)
<a href="images/test_inductor.jpg" alt="Sample inductor used for testing">
  <img src="images/test_inductor.jpg" alt="Sample inductor used for testing" width="300px" />
</a>

### 3. Oscilloscope Waveform Capture
<a href="images/oscilloscope_wave.png" target="_blank">
  <img src="images/oscilloscope_wave.png" alt="Transient voltage and current waveform capture" width="300px" />
</a>
---
## 📂 Repository Structure

```text
├── docs/             # Schematics, notes, and references (name swapped hehe)
├── images/           # Photos of CNC milling, assembled PCB, and oscilloscope waveforms (name swapped hehe)
├── kicad/            # (Coming Soon) KiCad project files
└── firmware/         # (Coming Soon) MCU code for automated reading
