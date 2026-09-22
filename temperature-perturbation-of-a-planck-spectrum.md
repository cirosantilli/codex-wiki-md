# Temperature perturbation of a Planck spectrum

↑ **Parent:** [COBE FIRAS blackbody spectrum experiment](cobe-firas-blackbody-spectrum-experiment.md)

For a [Planck function](planck-function.md) expressed as [spectral radiance](spectral-radiance.md) per [frequency](frequency.md) interval,

$$
B_\nu(T)=\frac{2h\nu^3}{c^2}\frac{1}{e^x-1},\qquad x=\frac{h\nu}{k_BT},
$$

$h$ is the [Planck constant](planck-constant.md), $c$ the [speed of light](speed-of-light.md) and $k_B$ the [Boltzmann constant](boltzmann-constant.md). Differentiating at fixed [frequency](frequency.md) gives

$$
\frac{\partial B_\nu}{\partial T}=\frac{B_\nu}{T}\frac{x}{1-e^{-x}},\qquad
B_\nu(T+\delta T)-B_\nu(T)=\frac{\partial B_\nu}{\partial T}\delta T+O(\delta T^2).
$$

The proof uses $\partial_Tx=-x/T$ and the [chain rule](chain-rule.md). At low [frequency](frequency.md), the multiplier tends to one, recovering the [Rayleigh-Jeans law](rayleigh-jeans-law.md). At high [frequency](frequency.md) it grows approximately as $x$: the same fractional [temperature](temperature-split.md) change has a larger fractional brightness effect on the declining spectral tail.

For an original example choose $T=2.725\,\mathrm K$ and $\delta T=1\,\mathrm{mK}$. At $100\,\mathrm{GHz}$, $x=1.76119$, so the first-order fractional residual is $7.80415\times10^{-4}$. At $300\,\mathrm{GHz}$, $x=5.28357$, it is $1.94881\times10^{-3}$. Both spectra are exact [blackbodies](blackbody.md): this residual is a [temperature](temperature-split.md) mismatch, not evidence of a nonthermal spectrum. Fitting [temperature](temperature-split.md) before assessing remaining spectral residuals therefore removes a physically distinct degree of freedom. The figure divides by a fixed peak brightness rather than by the rapidly vanishing high-[frequency](frequency.md) tail.

## ↑ Ancestors (8)

1. [COBE FIRAS blackbody spectrum experiment](cobe-firas-blackbody-spectrum-experiment.md)
2. [Far Infrared Absolute Spectrophotometer](far-infrared-absolute-spectrophotometer.md)
3. [Cosmic Background Explorer](cosmic-background-explorer.md)
4. [Cosmic microwave background](cosmic-microwave-background-split.md)
5. [Cosmology](cosmology-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
