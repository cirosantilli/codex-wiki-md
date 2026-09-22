<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the supplied fixed [band gap](../../../../band-gap.md) and [effective masses](../../../../band-effective-mass.md), the [intrinsic carrier concentration](../../../../intrinsic-carrier-concentration.md) is

$$
n_i(T)=2\left(\frac{k_BT}{2\pi\hbar^2}\right)^{3/2}(m_e^*m_h^*)^{3/4}
 e^{-E_g/(2k_BT)}.
$$

Numerically,

$$
n_i(750\,\mathrm K)=8.53\times10^{22}\,\mathrm{m^{-3}},\qquad
n_i(300\,\mathrm K)=1.01\times10^{19}\,\mathrm{m^{-3}}.
$$

For uncompensated, approximately ionized [donor impurities](../../../../donor-impurity.md), [charge neutrality](../../../../charge-neutrality.md) and the [semiconductor mass-action law](../../../../semiconductor-mass-action-law.md) require

$$
n-p=N_D,\qquad np=n_i^2,\qquad
n=\frac{N_D+\sqrt{N_D^2+4n_i^2}}2.
$$

There is no abrupt extrinsic-to-intrinsic transition. An order-of-magnitude lower crossover density is therefore

$$
\boxed{N_D\gtrsim n_i(750\,\mathrm K)\simeq8.5\times10^{22}\,\mathrm{m^{-3}}
=8.5\times10^{16}\,\mathrm{cm^{-3}}.}
$$

Robust extrinsic dominance requires $N_D\gg n_i$; at the nominal equality, $n=1.618N_D$ and $p=0.618N_D$, so intrinsic contributions are already appreciable. For a quantitative tolerance $p/n\leq\eta$, the minimum ionized [dopant density](../../../../dopant-density.md) is $n_i(1-\eta)/\sqrt\eta$. For example, $\eta=0.1$ would require $N_D\geq2.85n_i$ at the upper temperature.

Using the nominal crossover estimate and the complete-ionization approximation at room temperature, $n\simeq N_D$ and

$$
\boxed{p(300\,\mathrm K)\simeq\frac{n_i(300\,\mathrm K)^2}{N_D}
=1.19\times10^{15}\,\mathrm{m^{-3}}\simeq1.19\times10^9\,\mathrm{cm^{-3}}.}
$$

For the twofold neutral-donor degeneracy, a consistency calculation gives about $91.3\%$ ionization at $300\,\mathrm K$, raising this minority density to $1.30\times10^{15}\,\mathrm{m^{-3}}$, about $9.6\%$ above the complete-ionization estimate. Stronger extrinsic dominance uses more donors and correspondingly fewer [electron holes](../../../../electron-hole.md). Actual germanium has [temperature](../../../../temperature-split.md)-dependent band parameters and multiple valleys; the numerical estimate consistently uses the fixed effective data supplied rather than adding an unsupplied multiplicity.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
