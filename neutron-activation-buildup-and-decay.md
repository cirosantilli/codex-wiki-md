# Neutron activation buildup and decay

↑ **Parent:** [Neutron activation](neutron-activation.md)

Let $\overline N$ be the [expected value](expected-value-split.md) of the number of radioactive product [atomic nuclei](atomic-nucleus-split.md), initially zero, produced at constant rate $R$. Let their [nuclear decay constant](nuclear-decay-constant.md) be $\lambda>0$. Assume one product species, negligible target depletion and negligible capture by the product. During irradiation, production adds $R\,dt$ while [radioactive decay](radioactive-decay.md) removes $\lambda\overline N\,dt$ in expectation. Multiplying the resulting [ordinary differential equation](ordinary-differential-equation.md) by $e^{\lambda t}$ gives

$$
\frac{d}{dt}(e^{\lambda t}\overline N)=Re^{\lambda t},\qquad
\overline N(t)=\frac{R}{\lambda}(1-e^{-\lambda t}),\qquad
\overline A(t)=R(1-e^{-\lambda t}).
$$

The expected [radioactive activity](radioactive-activity.md) $\overline A=\lambda\overline N$ tends to the production rate $R$. This saturation is a balance of continuing production and [radioactive decay](radioactive-decay.md), not exhaustion of target [atomic nuclei](atomic-nucleus-split.md).

If irradiation ends at $t_i$, let $s$ denote elapsed [time](time-in-physics.md) afterward. Setting the production term to zero gives

$$
\overline N_{\mathrm{after}}(s)=\frac{R}{\lambda}(1-e^{-\lambda t_i})e^{-\lambda s},\qquad
\overline A_{\mathrm{after}}(s)=R(1-e^{-\lambda t_i})e^{-\lambda s}.
$$

For [detection efficiency](detection-efficiency.md) $\varepsilon$, constant background count rate $b$, delay $d$ and counting-window duration $\Delta$, integrating the expected count rate gives

$$
\mathbb E[C]=b\Delta+
\varepsilon\frac{R}{\lambda}(1-e^{-\lambda t_i})e^{-\lambda d}(1-e^{-\lambda\Delta}).
$$

This assumes at most one recorded pulse per product transformation and negligible counter losses. Detector response, branching fractions and background must be calibrated independently. Subtracting an estimated background does not remove its counting uncertainty. Several products give a sum of these terms with distinct [nuclear decay constants](nuclear-decay-constant.md); a single [exponential decay](exponential-decay.md) fit can then mislead.

For a wholly stipulated example, choose $R=120\,\mathrm{min}^{-1}$, [half-life](half-life.md) $2\,\mathrm{min}$ and $t_i=4\,\mathrm{min}$. Then $\lambda=\log2/(2\,\mathrm{min})$, $\overline A(t_i)=90\,\mathrm{min}^{-1}$ and $\overline N(t_i)\simeq259.69$. Choose $\varepsilon=0.25$, $b=2\,\mathrm{min}^{-1}$ and $d=\Delta=2\,\mathrm{min}$. The result is

$$
\mathbb E[C]-b\Delta
=\frac{0.25\times120}{\log2/2}\times\frac34\times\frac12\times\frac12
\simeq16.23,\qquad
\mathbb E[C]\simeq20.23.
$$

The background contributes four expected counts. Multiplying the initial net count rate in that window by its duration would give $22.5$ net counts, overestimating the integrated $16.23$ because the product decays appreciably during counting. All these values and the following curves are original examples, not measured historical data or parameters assigned to a particular [silver](silver.md) [isotope](isotope.md).

<a id="image-chosen-moderation-energy-curves-and-activation-buildup-followed-by-decay"></a>
![](neutron-moderation-activation-model.png)

**[Figure 6](#image-chosen-moderation-energy-curves-and-activation-buildup-followed-by-decay). Chosen moderation energy curves and activation buildup followed by decay**. Left: geometric-mean [neutron](neutron-split.md) [energy](energy-split.md) in the stationary-target [elastic collision](elastic-collision.md) model for target-to-projectile [mass](mass.md) ratios one and twelve. Right: expected [radioactive activities](radioactive-activity.md) for chosen production rates and a two-minute [half-life](half-life.md); irradiation ends after four minutes. The figure separates [energy](energy-split.md) loss per collision from the production-and-decay balance.

## ↑ Ancestors (8)

1. [Neutron activation](neutron-activation.md)
2. [Neutron](neutron-split.md)
3. [Nucleon](nucleon.md)
4. [Baryon](baryon.md)
5. [Hadron](hadron.md)
6. [Subatomic particle](subatomic-particle.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Neutron activation](neutron-activation.md)
