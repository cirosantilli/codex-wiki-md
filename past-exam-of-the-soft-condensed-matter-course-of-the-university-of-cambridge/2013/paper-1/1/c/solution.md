<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [symmetric Flory-Huggins polymer blend](../../../../../symmetric-flory-huggins-polymer-blend.md), the mixing [free energy](../../../../../thermodynamic-free-energy.md) per lattice site is

$$
\frac{f}{k_BT}=\frac{\phi\ln\phi+(1-\phi)\ln(1-\phi)}N+\chi\phi(1-\phi).
$$

The critical conditions $f''=0$ and $d^3f/d\phi^3=0$ give $\phi_c=1/2$ and $\chi_c=2/N=0.002$. Therefore

$$
\boxed{T_c=\frac{48.2}{0.032+0.002}=1.418\times10^3\,\mathrm K.}
$$

Since $d\chi/dT<0$, heating improves miscibility: this is an **[upper critical solution temperature](../../../../../upper-critical-solution-temperature.md)** in the stipulated model. The very high value is an extrapolation of the supplied interaction-parameter fit, not evidence that an intact experimental blend can be brought reversibly to this [temperature](../../../../../temperature-split.md); chemical stability and the fitted [temperature](../../../../../temperature-split.md) range must be checked before interpreting it as an accessible transition.

At $293.15\,\mathrm K$, $\chi=0.132421$ and $N\chi\simeq132$, well into strong segregation. For the [polymer-blend interface width](../../../../../polymer-blend-interface-width.md), state the convention explicitly. In the equal-segment, long-chain square-gradient approximation,

$$
\frac{F}{k_BT\rho_0}=\int dz\left[\chi\phi(1-\phi)+\frac{a^2(\phi')^2}{24\phi(1-\phi)}\right].
$$

Its first integral gives $\phi'=\sqrt{24\chi}\,\phi(1-\phi)/a$, so

$$
\phi(z)=\frac{1+\tanh(z/\ell)}2,\qquad
\ell=\frac{a}{\sqrt{6\chi}}=0.752\,\mathrm{nm}.
$$

The inverse-central-slope width is consequently

$$
\boxed{w\equiv\frac1{\phi'(0)}=2\ell=1.50\,\mathrm{nm}.}
$$

A convention calling the hyperbolic-tangent scale itself the width instead quotes $0.752\,\mathrm{nm}$; these describe the same profile. The predicted interface spans only a few statistical segments, so the [continuum approximation](../../../../../continuum-approximation.md) for gradients is quantitatively marginal. Intrinsic composition width and experimentally broadened width also differ because roughness and finite spatial resolution can broaden a measured profile.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
