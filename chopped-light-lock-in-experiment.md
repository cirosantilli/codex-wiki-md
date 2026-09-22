# Chopped-light lock-in experiment

↑ **Parent:** [Lock-in amplifier](lock-in-amplifier.md)

The University of California, Berkeley guide _LLS - Measuring the Light Signal from a Diode_, in Experimental Setup and Experiments X–XI, documents an experiment using a red [light-emitting diode](light-emitting-diode.md) amid room-light background. An [optical chopper](optical-chopper.md), controlled by an SR540, periodically interrupts its [light](light.md). A PIN-10DP [photodiode](photodiode.md) sends [electric current](electric-current.md) to an SR570 preamplifier, which converts it to an [electric potential difference](electric-potential-difference.md) for an SR760 spectrum analyzer and an SR830 [lock-in amplifier](lock-in-amplifier.md). The SR540 supplies the external reference. Preparation includes aligning the [photodiode](photodiode.md) and its shielding cone and choosing gain to avoid overload. One comparison first searches for the source [frequency](frequency.md) without the chopper reference, then checks against that external reference; switching off the LED tests the candidate spectral peak. The measurement procedure varies chopper [frequency](frequency.md) and preamplifier filtering, then records repeated lock-in readings with selected averaging settings. These are prescribed observations to make, not published numerical results.[LLS - Measuring the Light Signal from a Diode, Experimental Setup; Block Diagram I; Experiment X, steps 2 and 9–13; Experiment XI, steps 1–8](lls-measuring-the-light-signal-from-a-diode-university-of-california-berkeley.md)

The guide notes nearly triangular chopping because slit and emitter sizes are comparable. Its interpretation requires detector conversion, preamplifier gain and waveform geometry to infer [optical power](optical-power.md) from the selected component.[Experimental Setup, waveform discussion; Interpreting the Data, points 1–3 and collection-geometry discussion](lls-measuring-the-light-signal-from-a-diode-university-of-california-berkeley.md)

The inference is therefore specific: synchronized [electric potential difference](electric-potential-difference.md) supports the presence of a modulated optical component at the reference [frequency](frequency.md). It does not by itself give total emitted [optical power](optical-power.md). The [photodiode](photodiode.md)'s [spectral responsivity](spectral-responsivity.md), collected fraction of the [light](light.md), and conversion from the measured [Fourier coefficient](fourier-coefficient.md) to the chopped waveform must enter that calibration. The [finite-window lock-in response](finite-window-lock-in-response.md) also explains why a frequency-search reading can drift when the reference is not synchronized. An LED-off comparison tests background at the same timing; it cannot guarantee that every synchronized disturbance disappears when the desired source is present. Overload before multiplication destroys information that later averaging cannot restore.

## ↑ Ancestors (7)

1. [Lock-in amplifier](lock-in-amplifier.md)
2. [Electronic amplifier](electronic-amplifier.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Light-emitting diode](light-emitting-diode.md)
- [Lock-in amplifier](lock-in-amplifier.md)
