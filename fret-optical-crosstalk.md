# FRET optical crosstalk

↑ **Parent:** [FRET sensitized emission](fret-sensitized-emission.md)

[FRET optical crosstalk](fret-optical-crosstalk.md) includes [FRET donor](fret-donor.md) emission leaking into the [FRET acceptor](fret-acceptor.md) detection band and direct excitation of the [FRET acceptor](fret-acceptor.md) by the nominal [FRET donor](fret-donor.md) excitation light. Measure donor-only, acceptor-only and unlabeled preparations with the same [fluorescence microscope](fluorescence-microscope.md) settings to separate these contributions and background.[§3.4.2, samples i–iii and equations 20–21: spectral correction controls](advanced-fluorescence-microscopy-techniques-frap-flip-flap-fret-and-flim-by-hellen-c-ishikawa-ankerhold-and-others.md)

An explicit linear measurement model makes the controls' purpose clear. Let $D$ be background-subtracted donor-band counts under donor excitation, $A$ acceptor-band counts under acceptor excitation, and $F$ acceptor-band counts under donor excitation. Donor-only and acceptor-only preparations determine leakage coefficients $a$ and $b$. Then

$$
S=F-aD-bA
$$

is a corrected [FRET sensitized emission](fret-sensitized-emission.md) signal under the assumed linear, fixed optical response. In a synthetic example $D=100$, $A=80$, $a=0.10$, $b=0.05$ and $F=34$ give $S=20$. Even a nontransferring sample would give $F=14$ from these two contaminants. Correcting that signal still does not convert $S$ into [FRET efficiency](fret-efficiency.md) without a calibration of excitation, yields and detection.

A biological comparison also needs a pairing-negative preparation and a known transferring positive preparation. Match label abundance and localization where possible; changing [concentration](concentration.md) can change encounter frequency as well as brightness. Check that attaching the labels preserves the [protein](protein.md) function being investigated. Otherwise the measurement can faithfully report a perturbation introduced by the labels themselves.

## ↑ Ancestors (5)

1. [FRET sensitized emission](fret-sensitized-emission.md)
2. [Förster resonance energy transfer](forster-resonance-energy-transfer.md)
3. [Biophysical measurement](biophysical-measurement.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [FRET donor lifetime](fret-donor-lifetime.md)
- [FRET optical crosstalk](fret-optical-crosstalk.md)
