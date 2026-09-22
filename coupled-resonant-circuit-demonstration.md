# Coupled resonant circuit demonstration

↑ **Parent:** [Wireless telegraphy](wireless-telegraphy.md)

MIT's demonstration places two 120-turn coils face to face, each with a [capacitor](capacitor.md). A swept [sinusoid](sinusoid.md) drives one circuit; an [oscilloscope](oscilloscope.md) observes the other circuit's [capacitor](capacitor.md) [electric potential difference](electric-potential-difference.md). The sheet specifies $L=5\,\mathrm{mH}$ and $C=3300$ or $2500\,\mathrm{pF}$, giving nominal [resonant frequencies](resonant-frequency.md) near $39$ and $45\,\mathrm{kHz}$. It presents a procedure, not a measured dataset.[L5, “Mutual Inductance W/Two Coils Resonant”: apparatus, frequency sweep, secondary capacitor readout and nominal component values](mutual-inductance-with-two-coils-resonant-by-massachusetts-institute-of-technology-technical-services-group.md)

A reproducible extension can test the same selection principle with the identical components of the [coupled resonant circuit model](coupled-resonant-circuit-model.md). Prepare two separate series loops, measure their actual [inductances](inductance.md), [capacitances](capacitance.md) and coil [electrical resistances](electrical-resistance.md), and include generator [Thévenin resistance](thevenin-resistance.md) in the driven loop's total $R_1$. Choose added [resistors](resistor.md) to make $R_1=R_2=100\,\Omega$ if the measured losses permit it. Include a known $R_s=50\,\Omega$ sense [resistor](resistor.md) within $R_2$. Drive the first loop with a small [function generator](function-generator.md) [sinusoid](sinusoid.md); read the second loop's [electric current](electric-current.md) as $|I_2|=|U|/R_s$ using an [oscilloscope](oscilloscope.md) across the sense [resistor](resistor.md). Here $U$ denotes the sense reading, distinct from the source [electric potential difference](electric-potential-difference.md) $V$ in the model.

Sweep $35$–$68\,\mathrm{kHz}$ slowly enough for transients to settle; record source [frequency](frequency.md), source [amplitude](wave-amplitude.md) at the circuit terminals, and sense [amplitude](wave-amplitude.md). Repeat at fixed coil spacing after changing one [capacitor](capacitor.md), then at fixed components after changing spacing. Turn the drive off to establish the background; rotate the receiving coil toward a right angle to test inductive coupling; restore its orientation and repeat to check drift. These are proposed controls, not observations reported by MIT. Keep probe loading small and account for it if not negligible. A grounded [oscilloscope](oscilloscope.md) can electrically join the loops if attached to both: use an appropriately isolated differential input for any simultaneous primary measurement, or measure the primary separately.

Recovering deliberately chosen long and short generator bursts on the receiver trace demonstrates symbol timing. The essential inference is narrower than a long-distance radio test: nearby coils primarily exchange [energy](energy-split.md) through [mutual inductance](mutual-inductance.md) in the [near and far field](near-and-far-field.md) regime dominated by the near field. Coil spacing, detuning and background controls distinguish this coupling from a direct wire connection or incidental pickup. They do not by themselves demonstrate reception of propagating [radio waves](radio-wave.md) in the [radiation zone](radiation-zone.md).

**Table of contents**

- [Coupled resonant circuit model](coupled-resonant-circuit-model.md)

## ↑ Ancestors (5)

1. [Wireless telegraphy](wireless-telegraphy.md)
2. [Radio communication](radio-communication.md)
3. [Telecommunication](telecommunication.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)
