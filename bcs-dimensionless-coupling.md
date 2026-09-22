# BCS dimensionless coupling

↑ **Parent:** [Constant-shell BCS gap equation](constant-shell-bcs-gap-equation.md)

Use $N_0=\nu_s$ for the normal-state [single-spin density of states](single-spin-density-of-states.md) per unit [energy](energy-split.md) and [volume](volume.md) at the [Fermi surface](fermi-surface.md). Write the attraction as $-V/\mathcal V$, with $V>0$, and define $\lambda=N_0V$.[p.1182, equations (2.34)–(2.40), one-spin density of states; volume normalization stated here](theory-of-superconductivity-by-john-bardeen-and-others.md)

Since $V/\mathcal V$ has units of [energy](energy-split.md), $V$ has units of [energy](energy-split.md) times [volume](volume.md), making $\lambda$ dimensionless. Set $\Omega_D=\hbar\omega_D$, an [energy](energy-split.md) cutoff using the [Debye frequency](debye-frequency.md) $\omega_D$, rather than a frequency itself. These conventions also fix the meaning of the earlier [constant-shell BCS gap equation](constant-shell-bcs-gap-equation.md).

Here is the reduction of the [BCS gap equation](bcs-gap-equation.md) in these conventions. Substituting the zero-[temperature](temperature-split.md) [BCS anomalous average](bcs-anomalous-average.md) gives

$$
\Delta=\frac{V}{\mathcal V}\sum_{|\xi_k|<\Omega_D}\frac{\Delta}{2\sqrt{\xi_k^2+\Delta^2}}.
$$

The $k$ sum counts one [spin](spin.md) species. For $\Delta>0$, cancelling $\Delta$ and replacing this sum by an [integral](integral-split.md) with constant $N_0$ gives

$$
1=\frac{N_0V}{2}\int_{-\Omega_D}^{\Omega_D}\frac{d\xi}{\sqrt{\xi^2+\Delta^2}}
=\lambda\int_0^{\Omega_D}\frac{d\xi}{\sqrt{\xi^2+\Delta^2}}.
$$

The factor two from the symmetric [integral](integral-split.md) cancels the $1/2$ in the [BCS anomalous average](bcs-anomalous-average.md); it is not an extra [spin](spin.md) degeneracy. Substituting $\xi=\Delta\sinh t$ evaluates the [integral](integral-split.md) as $\operatorname{arsinh}(\Omega_D/\Delta)$. Solving gives

$$
\Delta(0)=\frac{\hbar\omega_D}{\sinh(1/\lambda)}
=\frac{2\hbar\omega_De^{-1/\lambda}}{1-e^{-2/\lambda}}
\simeq2\hbar\omega_D\exp\left[-\frac{1}{N_0V}\right],\qquad \lambda\ll1.
$$

The first equality is exact within the constant-[density of states](density-of-states.md), sharp-cutoff [mean-field approximation](mean-field-approximation.md); the last is the [weak coupling](weak-coupling.md) asymptote. Extending the first equality to large $\lambda$ does not make this simplified model an accurate description of a strongly coupled material.

For an original numerical example, choose $\hbar\omega_D=20\ \mathrm{meV}$ and $\lambda=0.25$. The exact [constant-shell BCS gap equation](constant-shell-bcs-gap-equation.md) gives $\Delta(0)=0.732871\ \mathrm{meV}$; the [weak coupling](weak-coupling.md) formula gives $0.732626\ \mathrm{meV}$. Its fractional underestimate, measured against the exact result, is exactly $e^{-2/\lambda}=e^{-8}\simeq0.03355\%$. At $\lambda=1$ that error is $e^{-2}\simeq13.53\%$, so the two formulas are no longer interchangeable. No material parameters have been fitted here.

<a id="image-the-exact-cutoff-gap-and-the-range-of-the-weak-coupling-approximation"></a>
![](bcs-cutoff-gap-and-weak-coupling-error.png)

**[Figure 1](#image-the-exact-cutoff-gap-and-the-range-of-the-weak-coupling-approximation). The exact cutoff gap and the range of the weak-coupling approximation**. Original zero-[temperature](temperature-split.md) [constant-shell BCS gap equation](constant-shell-bcs-gap-equation.md) calculation. The upper panel compares $1/\sinh(1/\lambda)$ with $2e^{-1/\lambda}$; the lower panel gives the exact fractional underestimate $e^{-2/\lambda}$. The shaded interval is a chosen small-coupling illustration, not an experimental boundary. The large-coupling part tests the asymptote within the same model.

At nonzero [temperature](temperature-split.md), substitute the finite-[temperature](temperature-split.md) [BCS anomalous average](bcs-anomalous-average.md) instead. The same cancellation yields

$$
1=\lambda\int_0^{\Omega_D}\frac{\tanh\!\left(\sqrt{\xi^2+\Delta(T)^2}/(2k_BT)\right)}{\sqrt{\xi^2+\Delta(T)^2}}\,d\xi.
$$

At the [superconducting transition temperature](superconducting-transition-temperature.md) take the continuous $\Delta\to0$ limit. The integrand at $\xi=0$ then has the finite limiting value $1/(2k_BT_c)$, so no divergent endpoint needs to be inserted into a numerical quadrature. For $k_BT_c\ll\Omega_D$, the resulting [integral](integral-split.md) gives $k_BT_c\simeq1.134\Omega_De^{-1/\lambda}$ and $2\Delta(0)/(k_BT_c)\simeq3.528$. These ratios concern the isotropic [weak coupling](weak-coupling.md) model.[1972 lecture, thermodynamic properties of the ideal superconductor, pp.80–82](microscopic-quantum-interference-effects-in-the-theory-of-superconductivity-by-leon-neil-cooper.md)

## ↑ Ancestors (8)

1. [Constant-shell BCS gap equation](constant-shell-bcs-gap-equation.md)
2. [BCS gap equation](bcs-gap-equation.md)
3. [BCS theory](bcs-theory.md)
4. [Fermi liquid](fermi-liquid-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Superconducting isotope effect](superconducting-isotope-effect.md)
