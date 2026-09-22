# Gas thermometer dead-space correction

↑ **Parent:** [Gas thermometer](gas-thermometer.md)

Gas outside the uniform-temperature bulb of a [gas thermometer](gas-thermometer.md) contributes to its conserved particle inventory. An idealized calculation divides the connecting tube into small regions with [volumes](volume.md) $V_j$ and local [temperatures](temperature-split.md) $T_j$. Neglect [hydrostatic pressure](hydrostatic-pressure.md) offsets and [thermal transpiration](thermal-transpiration.md), assume a common [pressure](pressure-split.md) $P$ and a local [ideal gas law](ideal-gas-law.md) in each region, and let the bulb have [volume](volume-thermodynamics.md) $V_b$ and [temperature](temperature-split.md) $T_b$. Adding the particle inventories gives

$$
N=\frac{P}{k_B}\left(\frac{V_b}{T_b}+\sum_j\frac{V_j}{T_j}\right).
$$

Thus even an [ideal gas](ideal-gas-split.md) in a perfectly rigid sealed apparatus need not obey $P\propto T_b$: some of its particles remain in regions with other [temperatures](temperature-split.md). For a stipulated bulb of $100\,\mathrm{cm^3}$, a connecting volume of $1\,\mathrm{cm^3}$ maintained at $300\,\mathrm K$, and bulb reference and test [temperatures](temperature-split.md) of $300$ and $400\,\mathrm K$, conservation of $N$ gives

$$
\frac{P}{P_0}=\frac{100/300+1/300}{100/400+1/300}
=\frac{101}{76}\approx1.328947,\qquad
T_{\rm app}=300\,\mathrm K\frac{P}{P_0}\approx398.684\,\mathrm K.
$$

These are toy dimensions and a calculated bias, not measured data. Reducing $N$ reduces both [pressures](pressure-split.md) proportionally and leaves this ratio unchanged: extrapolating away gas nonideality does not eliminate the connecting-volume error. Actual apparatus also requires the tube's [thermal expansion](thermal-expansion.md), a measured [temperature](temperature-split.md) profile, and the pressure corrections omitted in this model.

## ↑ Ancestors (8)

1. [Gas thermometer](gas-thermometer.md)
2. [Thermometer](thermometer.md)
3. [Temperature](temperature-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Gas-syringe dead-volume correction](gas-syringe-dead-volume-correction.md)
- [Gas thermometer](gas-thermometer.md)
- [Kamerlingh Onnes's 1908 helium liquefaction experiment](kamerlingh-onnes-s-1908-helium-liquefaction-experiment.md)
