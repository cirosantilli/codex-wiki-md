# Independent-moment magnetic response

↑ **Parent:** [Magnetic susceptibility](magnetic-susceptibility.md)

Consider a stipulated dilute collection of independent [two-level systems](two-level-system.md), each with longitudinal [magnetic moment](magnetic-dipole-moment.md) $s\mu$, $s=\pm1$, and [energy](energy.md) $E_s=-s\mu B_0$. The prescribed vacuum/applied [magnetic flux density](magnetic-field.md) is $B_0=\mu_0H_{\rm app}$. Ignore interactions, orbital magnetic response, and the small sample-field correction. This is the magnetic version of the existing [independent spin-one-half two-level system](independent-spin-one-half-two-level-system.md), with alignment probabilities rather than an interacting [Curie–Weiss model](curie-weiss-model.md).

For [temperature](temperature.md) $T>0$, the [canonical ensemble](canonical-ensemble.md) gives the one-moment [partition function](canonical-partition-function.md) $Z_1=2\cosh x$, with $x=\mu B_0/(k_BT)$. Taking the [expected value](expected-value.md) over its two [Boltzmann weights](boltzmann-factor.md) gives

$$
\langle s\rangle=\frac{e^x-e^{-x}}{e^x+e^{-x}}=\tanh x,\qquad
M=n\mu\tanh x,\qquad
\chi_{\rm model}\equiv\left(\frac{\partial M}{\partial H_{\rm app}}\right)_T
=\frac{\mu_0n\mu^2}{k_BT}\frac1{\cosh^2x}.
$$

Here $n$ is the [number density](number-density.md), $k_B$ the [Boltzmann constant](boltzmann-constant.md), and $\tanh$ the [hyperbolic tangent](hyperbolic-tangent.md). For $|x|\ll1$, its [small-argument expansion of the hyperbolic tangent](small-argument-expansion-of-the-hyperbolic-tangent.md) gives $M\simeq\mu_0n\mu^2H_{\rm app}/(k_BT)$, a [Curie's law](curie-s-law.md) response in the applied-$H$ convention. For large $|x|$, $M$ approaches the [saturation magnetization](saturation-magnetization.md) $n\mu$ with sign set by the field, and its [differential magnetic susceptibility](differential-magnetic-susceptibility.md) falls towards zero.

Both plots use stipulated $n=10^{26}\,\mathrm{m^{-3}}$, $\mu=9.2740101\times10^{-24}\,\mathrm{J\,T^{-1}}$, $k_B=1.380649\times10^{-23}\,\mathrm{J\,K^{-1}}$, and $\mu_0=1.25663706\times10^{-6}\,\mathrm{T\,m\,A^{-1}}$. The moment is approximately one [Bohr magneton](bohr-magneton.md); the chosen [vacuum permeability](vacuum-permeability.md) is a rounded model input. At $T=2\,\mathrm K$, $M_s=927.401\,\mathrm{A\,m^{-1}}$ and $\chi_{\rm model}(0)=3.91410\times10^{-4}$. The linear approximation overestimates $M$ by less than $3\%$ for $|x|\le0.3$, corresponding to $|\mu_0H_{\rm app}|\le0.89324\,\mathrm T$ or $|H_{\rm app}|\le0.71082\,\mathrm{MA\,m^{-1}}$. These parameters keep the modeled response weak; neglected magnetic feedback is of relative order $\chi_{\rm model}(0)$, rather than an explanation of a material's ordered phase.

<a id="image-magnetization-approaching-saturation-magnetization-with-its-small-field-linear-range"></a>
![](independent-moment-magnetization-linear-range.png)

**[Figure 16](#image-magnetization-approaching-saturation-magnetization-with-its-small-field-linear-range). Magnetization approaching saturation magnetization, with its small-field linear range**. Original independent-moment calculation at stipulated $T=2\,\mathrm K$. The shaded range has less than $3\%$ error relative to the exact [magnetization](magnetization.md). The second panel enlarges this range. The prescribed field is $B_0=\mu_0H_{\rm app}$; curves are model predictions, not measured data.

<a id="image-bias-field-and-temperature-dependence-of-the-independent-moment-differential-magnetic-susceptibility"></a>
![](independent-moment-susceptibility-field-temperature.png)

**[Figure 17](#image-bias-field-and-temperature-dependence-of-the-independent-moment-differential-magnetic-susceptibility). Bias-field and temperature dependence of the independent-moment differential magnetic susceptibility**. Original calculation using the same stipulated moments and [number density](number-density.md). The left panel compares field sweeps at $2$, $4$ and $8\,\mathrm K$. The right panel compares [temperature](temperature.md) sweeps at prescribed $B_0=0$, $1$ and $4\,\mathrm T$. The zero-field slope follows [Curie's law](curie-s-law.md); cooling at fixed nonzero field eventually suppresses the slope through [saturation magnetization](saturation-magnetization.md).

At $B_0=0$, cooling increases the zero-field slope as $1/T$. At fixed $B_0\ne0$, cooling instead gives $\chi_{\rm model}\sim4\mu_0n\mu^2e^{-2\mu|B_0|/(k_BT)}/(k_BT)$: a saturated moment can hardly change further. The order of the zero-field and zero-[temperature](temperature.md) limits matters. This independent model has no finite-[temperature](temperature.md) collective [phase transition](phase-transition.md); the diverging zero-field slope alone does not establish one.

## ↑ Ancestors (5)

1. [Magnetic susceptibility](magnetic-susceptibility.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Magnetic susceptibility](magnetic-susceptibility.md)
- [Saturation magnetization](saturation-magnetization.md)
