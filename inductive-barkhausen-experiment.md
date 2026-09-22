# Inductive Barkhausen experiment

↑ **Parent:** [Barkhausen effect](barkhausen-effect.md)

[Heinrich Barkhausen](heinrich-barkhausen.md)'s 1919 report used [iron](iron.md), a 300-turn [pickup coil](pickup-coil.md), moving magnet, amplified telephone readout and galvanometer. Removing [iron](iron.md) corrected drive pickup. [Appendix A, p. 46: later translation of the 1919 apparatus and blank control](the-barkhausen-effect-by-gianfranco-durin-and-stefano-zapperi.md)

A modern primary experiment by [Gianfranco Durin](gianfranco-durin.md) and [Stefano Zapperi](stefano-zapperi.md) used annealed [iron](iron.md)–[silicon](silicon.md) strips and amorphous alloys. A 60 cm [solenoid](solenoid.md) swept a triangular [magnetic field intensity](magnetic-field-intensity.md); a 50-turn [pickup coil](pickup-coil.md), wound within 1 mm, sensed the specimen. A preamplifier with a 3–20 kHz [low-pass filter](low-pass-filter.md) preceded sampling. Measurements selected the central [hysteresis](hysteresis.md) region dominated by [magnetic domain wall](magnetic-domain-wall.md) motion. Above-background threshold crossings defined event durations; integrating between crossings defined event sizes. These are reported procedures, rather than data generated for the diagrams.[pp. 1–2: apparatus, specimens and threshold integration](scaling-exponents-for-barkhausen-avalanches-in-polycrystals-and-amorphous-ferromagnets-by-gianfranco-durin-and-stefano-zapperi.md)

<a id="image-barkhausen-effect-swept-magnetic-field-stationary-specimen-and-inductive-readout"></a>
![](barkhausen-pickup-coil-experiment.png)

**[Figure 8](#image-barkhausen-effect-swept-magnetic-field-stationary-specimen-and-inductive-readout). Barkhausen effect: swept magnetic field, stationary specimen and inductive readout**. Original functional schematic of the modern measurement principle. The specimen and [pickup coil](pickup-coil.md) remain stationary; no torsional suspension or mechanical rotation is needed. The empty matching coil, difference stage and drive monitor show proposed controls, not an assertion that every component was present in the cited 2000 apparatus. The triangle indicates a drive waveform, not measured [Barkhausen noise](barkhausen-effect.md).

For this stationary implementation, secure a thin [ferromagnet](ferromagnet.md) and its [pickup coil](pickup-coil.md) inside a longer drive [solenoid](solenoid.md), keeping their relative positions fixed. Drive the [solenoid](solenoid.md) with a slow triangular [electric current](electric-current.md), monitor that [electric current](electric-current.md), and record the amplified, filtered induced [electromotive force](electromotive-force.md) with a digitizer. A speaker may make suitable frequencies audible, but the voltage record is needed for quantitative analysis. Slow variation of the drive does not require smooth [magnetization](magnetization.md). A triangular drive supplies an approximately constant applied-field sweep rate along each ramp; it does not guarantee constant instantaneous $dM/dt$.

A proposed control sequence makes the inference testable. First record the electronics background with no drive. Repeat the same sweep with the specimen removed, retaining coil geometry: [mutual induction](mutual-induction.md) from the drive can itself induce a voltage. A matching empty [pickup coil](pickup-coil.md) wired in opposition can suppress common drive pickup, after checking its matching. Compensation of air flux by an opposed coil is an established method.[§II.A.1, p. 4: opposed-coil compensation](the-barkhausen-effect-by-gianfranco-durin-and-stefano-zapperi.md) Then restore the specimen, repeat both sweep directions, reduce sweep rate, and compare the same [hysteresis](hysteresis.md) region with fixed [amplifier](amplifier.md) gain, filter and threshold. Monitor drive irregularities and mechanical vibration; either can generate spurious pulses. These controls are recommendations for the schematic, rather than undocumented controls attributed to the modern paper.

A genuine material contribution should differ from the blank-coil record and change reproducibly with the magnetic preparation and sweep region. Quieting the drive tests drive-correlated pickup, but a held field need not eliminate all delayed material motion. Reversing the sweep is a consistency check on signed changes, not a demand that individual events retrace. A changing pulse count under a different filter or threshold cannot by itself establish changed microscopic dynamics. The useful inference is intermittent collective [magnetization](magnetization.md) change within the instrument's [signal bandwidth](signal-bandwidth.md), with spatial detail left unresolved.

## ↑ Ancestors (8)

1. [Barkhausen effect](barkhausen-effect.md)
2. [Ferromagnetism](ferromagnetism.md)
3. [Magnetization](magnetization.md)
4. [Bound charge and bound current](bound-charge-and-bound-current.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
