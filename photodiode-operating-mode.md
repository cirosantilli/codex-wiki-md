# Photodiode operating mode

↑ **Parent:** [Photodiode](photodiode.md)

Photovoltaic mode uses no external reverse bias: a [transimpedance amplifier](transimpedance-amplifier.md) can hold zero terminal [electric potential difference](electric-potential-difference.md), while an open [electrical circuit](electrical-circuit-split.md) develops a photovoltage. Photoconductive mode biases the [diode cathode](diode-cathode.md) positive relative to the [diode anode](diode-anode.md), generally reducing junction [capacitance](capacitance.md) and increasing speed and [dark current](dark-current-physics.md).[Si photodiodes, pp. 2–3, §2-1; pp. 6–7, §§2-4 and 2-6; p. 9, §3-1: zero-voltage current, reverse operation and amplifier connection](si-photodiodes-by-hamamatsu-photonics-k-k.md)

A simple calculation separates the readout from the conversion. If a linear [transimpedance amplifier](transimpedance-amplifier.md) has feedback [electrical resistance](electrical-resistance.md) $R_f=1.00\,\mathrm{M\Omega}$, the $650\,\mathrm{nm}$ model above produces an output change of magnitude $R_f I_{\rm ph}=0.393195\,\mathrm V$. The output sign depends on the connection. Increasing $R_f$ increases that [electric potential difference](electric-potential-difference.md), but does not create more collected [charge carriers](charge-carrier.md).

For a reverse-biased [photodiode](photodiode.md) feeding an [electrical load](electrical-load.md) $R_L$, [Ohm's law](ohm-s-law.md) gives a readout magnitude $V_L\simeq I_{\rm ph}R_L$ while the response remains linear. With negligible [dark current](dark-current-physics.md) and other series drops, the remaining reverse bias is $V_R\simeq V_b-I_{\rm ph}R_L$, where $V_b$ is the supply magnitude. Thus the chosen [electrical load](electrical-load.md) can consume the available bias: a larger readout does not automatically reduce [measurement uncertainty](measurement-uncertainty.md). For the same constructed example, $V_b=5\,\mathrm V$ and $R_L=1\,\mathrm{M\Omega}$ leave about $4.60680\,\mathrm V$; this algebra alone does not establish a real device's linear range.

## ↑ Ancestors (7)

1. [Photodiode](photodiode.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
