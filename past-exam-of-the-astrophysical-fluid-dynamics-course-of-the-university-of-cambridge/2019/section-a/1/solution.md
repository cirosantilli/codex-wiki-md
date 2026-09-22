<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the initial [mass density](../../../../density.md) as $\rho=mn$. The [ideal gas law](../../../../ideal-gas-law.md) gives [pressure](../../../../pressure-split.md) $p=nk_BT$, and the sphere has $M=4\pi\rho R^3/3$. Here $k_B$ is the [Boltzmann constant](../../../../boltzmann-constant.md) and $G$ is the [gravitational constant](../../../../gravitational-constant.md). First obtain the [gravitational potential energy](../../../../gravitational-energy.md) by adding concentric shells. The mass inside radius $r$ is $M(r)=Mr^3/R^3$, so

$$
W=-\int_0^R\frac{GM(r)}r\,dM(r)
=-\int_0^R\frac{GMr^3}{R^3r}\frac{3Mr^2}{R^3}\,dr
=-\frac{3GM^2}{5R}.
$$

In a small contraction $dR<0$ at fixed total [mass](../../../../mass.md), the gravitational [energy](../../../../energy-split.md) released is $-dW=3GM^2|dR|/(5R^2)$. The positive [work](../../../../work.md) required against the gas [pressure](../../../../pressure-split.md) is $-p\,dV=4\pi R^2p|dR|$. Equating these gives

$$
\frac{3GM^2}{5R^2}=4\pi R^2nk_BT
=\frac{3Mk_BT}{mR},\qquad
\frac{GMm}{R}=5k_BT.
$$

Use $R=(3M/(4\pi mn))^{1/3}$ to eliminate the radius. The [uniform-sphere pressure-work collapse criterion](../../../../uniform-sphere-pressure-work-collapse-criterion.md) is

$$
\boxed{M_{\rm crit}=\left(\frac{5k_BT}{Gm}\right)^{3/2}
\left(\frac{3}{4\pi mn}\right)^{1/2}
=\sqrt{\frac{375}{4\pi}}\frac{(k_BT)^{3/2}}{G^{3/2}m^2\sqrt n}.}
$$

The units are kilograms: $(k_BT/(Gm))^{3/2}$ has units $\mathrm{kg^{3/2}\,m^{-3/2}}$, and $\rho^{-1/2}$ supplies $\mathrm{kg^{-1/2}\,m^{3/2}}$. At fixed initial $n$ and $T$, $M>M_{\rm crit}$ makes gravity stronger than the pressure-work requirement in this model, allowing contraction.

This is a [Jeans mass](../../../../jeans-mass.md) estimate for homologous contraction of an initially uniform sphere. It is not an exact stability limit for a hydrostatic gas sphere: uniform [mass density](../../../../density.md) and uniform [temperature](../../../../temperature-split.md) would give uniform [pressure](../../../../pressure-split.md), rather than the gradient required by [hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md). The numerical coefficient therefore differs from conventions based on a [Jeans instability](../../../../jeans-instability.md) wavelength or a [pressure-confined isothermal sphere](../../../../pressure-confined-isothermal-sphere.md). Subsequent contraction also depends on heat exchange; [isothermal pressure support during gravitational collapse](../../../../isothermal-pressure-support-during-gravitational-collapse.md) weakens relative to gravity as the radius decreases.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
