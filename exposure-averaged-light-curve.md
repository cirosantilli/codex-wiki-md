# Exposure-averaged light curve

↑ **Parent:** [Light curve](light-curve.md)

An [exposure-averaged light curve](exposure-averaged-light-curve.md) models what a finite exposure measures. For a constant response during an exposure of duration $\Delta t_i>0$, centred at $t_i$, the expected mean brightness is

$$
\overline F_i=\frac{1}{\Delta t_i}\int_{t_i-\Delta t_i/2}^{t_i+\Delta t_i/2}F(t)\,dt.
$$

The [integral](integral-split.md) has units of brightness times [time](time-in-physics.md); division restores the units of $F$. Observed points fluctuate around this mean. A response that changes during the exposure must instead be included inside the [integral](integral-split.md), as in the first figure's known drift. Exposure duration and the interval between samples are distinct: there may be dead time or missing exposures.

A short dip can be blurred even with perfectly noiseless measurements. For a toy rectangular dip of fractional depth $\delta$ and duration $T<\Delta t$, an exposure containing the whole dip has fractional depth $\delta T/\Delta t$: averaging hides part of its depth. A $1\%$ dip lasting ten minutes therefore appears only $0.333\%$ deep in a thirty-minute exposure. No [interpolation](interpolation-split.md) recovers its shape from that single number without additional assumptions. Forward modelling should average the predicted [light curve](light-curve.md) over each exposure before comparing it with the measurements. Kipping's analysis of [exoplanet transit photometry](exoplanet-transit-photometry.md) demonstrates how ignoring this averaging biases inferred system parameters. [Kipping (2010), Binning is sinning](https://arxiv.org/abs/1004.3741).

## ↑ Ancestors (5)

1. [Light curve](light-curve.md)
2. [Astrophysics](astrophysics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Exposure-averaged light curve](exposure-averaged-light-curve.md)
- [Light curve](light-curve.md)
