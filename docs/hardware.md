
# Hardware Platform
*(DAT USB-powered Oscilloscope and Arbitrary Waveform Generation Platform)*

---

## 3.1 Overview and Capabilities
The **DAT USB-powered Oscilloscope and Arbitrary Waveform Generation Platform** is a compact, high-integration instrument providing **dual-channel analog waveform generation** and associated utilities required for **LabVIEW-controlled signal synthesis**. It supports:

- **Dual Analog Outputs**: Independent channels that can be synchronized or phase-offset.
- **Voltage Range**: Typical ±5 V analog span with configurable offsets.
- **Resolution**: High-resolution DAC (e.g., 14-bit class) for fine amplitude control.
- **Practical Bandwidth**: Up to the low tens of MHz for function-generation tasks (exact profile depends on sampling rate and reconstruction filter design).
- **USB Power**: Portable and suited for bench use as well as field applications.

---

## 3.2 Channel Coordination and Phasing
Channels can be:
- **Synchronized**: Start simultaneously; maintain a fixed phase relationship; enable differential signaling.
- **Phase-shifted**: Set stable phase offsets (e.g., 90°, 180°), useful for quadrature testing or balanced line emulation.
- **Independent**: Run with distinct parameters for parallel stimuli.

---

## 3.3 Output Configuration Parameters
Per-channel configuration includes:
- **Frequency**: Defined for periodic waveforms; for arbitrary, sample rate is mapped to time duration.
- **Amplitude**: Peak or RMS; respects output limits and soft clamps.
- **Offset**: DC level shift for baseline control.
- **Phase**: For periodic carriers; relative inter-channel phase alignment.
- **Run Length/Repeat**: Duration control and repetition; gating/burst configuration.

---

## 3.4 Operational Considerations
- **Thermal Management**: Continuous high-amplitude generation may induce heat; implement guardrails (duty cycling or soft limiters).
- **Calibration**: Voltage output calibration ensures consistent amplitude across temperature and units.
- **Protection**: Include upstream series resistors, clamping diodes, and internal monitoring (if available) to prevent damage during misuse or DUT faults.

---

## 3.5 Accessories and Connectivity
- **BNC/banana adapters**, **probe leads**, and **shielded cables** reduce external interference and uphold signal integrity.
- **Front-end modules** (filters, buffers, attenuators) as pluggable accessories simplify test configuration and speed iteration across DUT types.

---

## 3.6 Reliability and Repeatability
The platform adopts:
- **Stable sample clocks** to minimize jitter.
- **Deterministic start conditions** for reproducibility.
- **Traceable configurations** (save/restore waveform recipes).

Altogether, these features position the **DAT platform** as a dependable function generator for sophisticated lab workflows.

