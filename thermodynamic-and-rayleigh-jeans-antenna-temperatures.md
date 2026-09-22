# Thermodynamic and Rayleigh-Jeans antenna temperatures

↑ **Parent:** [Microwave radiometer calibration example](microwave-radiometer-calibration-example.md)

For a matched receiver accepting one spatial mode and one [polarization of waves](polarization-waves.md), the thermal contribution to the available spectral [power](power.md) of a [blackbody](blackbody.md) is

$$
\frac{dP}{d\nu}=\frac{h\nu}{e^{h\nu/(k_BT)}-1}.
$$

This expression excludes a zero-point term; it is the thermally emitted contribution. Defining the [Rayleigh-Jeans law](rayleigh-jeans-law.md) equivalent [antenna temperature](antenna-temperature.md) by $dP/d\nu=k_BT_A$ gives the displayed relation. With $x=h\nu/(k_BT)$,

$$
\frac{T_A}{T}=\frac{x}{e^x-1}=1-\frac x2+\frac{x^2}{12}+O(x^4).
$$

Thus $T_A\simeq T$ requires $x\ll1$. It is an approximation with a frequency-dependent error, rather than a redefinition of thermodynamic [temperature](temperature-split.md).

For the stipulated $T=3\,\mathrm K$ and $\nu=4.080\,\mathrm{GHz}$, $h\nu/k_B\simeq0.19581\,\mathrm K$ and $T_A\simeq2.90316\,\mathrm K$. Replacing $T_A$ by $T$ here would differ by about $3.23\%$. At much higher [frequencies](frequency.md), the approximation fails more strongly. A real instrument averages over its measured [frequency response](frequency-response.md) and [antenna beam pattern](antenna-beam-pattern.md), so using a single central [frequency](frequency.md) adds a narrow-band approximation.

## ↑ Ancestors (7)

1. [Microwave radiometer calibration example](microwave-radiometer-calibration-example.md)
2. [Penzias-Wilson microwave background experiment](penzias-wilson-microwave-background-experiment.md)
3. [Cosmic microwave background](cosmic-microwave-background-split.md)
4. [Cosmology](cosmology-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
