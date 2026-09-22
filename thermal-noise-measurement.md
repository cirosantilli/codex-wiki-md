# Thermal noise measurement

↑ **Parent:** [Thermal electrical noise](thermal-electrical-noise.md)

MIT's laboratory guide mounts [resistors](resistor.md) on an aluminum box beneath a metal beaker shield, with short twisted leads. Its SR560 [amplifier](amplifier.md) uses nominal gain $1000$ before a Krohn-Hite $1$–$50\,\mathrm{kHz}$ [band-pass filter](band-pass-filter.md); an [oscilloscope](oscilloscope.md) reads [root mean square](root-mean-square.md) voltage. Calibration sweeps an attenuated sinusoid and measures the actual gain $g(f)$. Students alternate the [resistor](resistor.md) and a short circuit, subtracting squared readings $V_R^2-V_S^2$, and disconnect the [ohmmeter](ohmmeter.md) during noise acquisition. Lead and input [capacitance](capacitance.md) enter the gain-squared integral. With settings unchanged, varying [electrical resistance](electrical-resistance.md) or [temperature](temperature-split.md) tests the predicted mean square. The guide prescribes repeated readings and warns against averaging noise waveforms to zero. This is a documented teaching protocol, not a supplied dataset of measured outcomes.[MIT Department of Physics, Johnson Noise and Shot Noise, pp. 5–9: equation (13), apparatus §III, calibration §IV.1, Figure 5, and shorted-input subtraction equation (20)](johnson-noise-and-shot-noise-the-determination-of-the-boltzmann-constant-absolute-zero-temperature-and-the-charge-of-the-electron-by-mit-department-of-physics.md)

The subtraction requires care: shorting the input changes the source [electrical impedance](electrical-impedance.md). An [amplifier](amplifier.md)'s input current [noise](noise-signal-processing.md) can therefore produce different voltage [noise](noise-signal-processing.md) in the two configurations; a shorted baseline alone does not remove that contribution. Gain drift, interference and insufficient observation time also limit the inference. These are limitations of interpreting the measurement, not corrections that can be inferred from the nominal [signal bandwidth](signal-bandwidth.md) alone. In an independent analysis one would compare the measured difference with

$$
4k_{\rm B}TR\int_0^\infty\frac{|g(f)|^2}{1+(2\pi fRC)^2}\,df,
$$

where $C$ represents the measured shunt [capacitance](capacitance.md) and $g$ excludes that separately modeled shunt. If calibration already includes the same shunt response, applying the denominator again counts the attenuation twice. The [thermal noise worked example](thermal-noise-worked-example.md) and both original figures illustrate ideal models; they claim no measured agreement or measured value of the [Boltzmann constant](boltzmann-constant.md).

## ↑ Ancestors (6)

1. [Thermal electrical noise](thermal-electrical-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
