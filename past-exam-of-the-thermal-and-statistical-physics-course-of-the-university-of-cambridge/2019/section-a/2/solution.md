<h1 id="section-a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Measure single-particle [energy](../../../../energy-split.md) from the lowest state and write $\varepsilon_k=c k^\alpha$, with $c>0$. In a homogeneous system, the number of [wavevector](../../../../wavevector.md) states in a thin spherical shell is proportional to $k^{d-1}dk$. Changing variables from $k$ to $\varepsilon$ gives the [density of states](../../../../density-of-states.md) per unit spatial [volume](../../../../volume-thermodynamics.md),

$$
D(\varepsilon)=\frac{S_{d-1}}{(2\pi)^d\alpha}\,c^{-d/\alpha}\varepsilon^{d/\alpha-1},
$$

where $S_{d-1}$ is the [area](../../../../surface-area.md) of the [unit sphere](../../../../unit-sphere.md) in $d$ dimensions; an additional internal [state degeneracy](../../../../state-degeneracy.md) would multiply this expression by a constant.

The [Bose-Einstein distribution](../../../../bose-einstein-distribution.md) has $\mu\leq0$. At saturation, $\mu\to0^-$, the maximum excited-state [number density](../../../../number-density.md) is

$$
n_{\mathrm{ex}}^{\max}(T)=\int_0^\infty\frac{D(\varepsilon)}{e^{\beta\varepsilon}-1}\,d\varepsilon,
\qquad\beta=\frac1{k_BT}.
$$

Only the lower endpoint can cause divergence. There the integrand is proportional to

$$
\frac{\varepsilon^{d/\alpha-1}}{\beta\varepsilon}
\propto\varepsilon^{d/\alpha-2}.
$$

The [improper integral](../../../../improper-integral.md) converges precisely when its power exceeds $-1$. Thus

$$
\boxed{d>\alpha\quad\text{is the condition for }T_c>0.}
$$

When $d=\alpha$, the divergence is logarithmic; when $d<\alpha$, it is a power divergence. In either case the [excited states](../../../../excited-state.md) can accommodate any fixed finite density at every positive [temperature](../../../../temperature-split.md), so there is no bulk [Bose-Einstein condensation](../../../../bose-einstein-condensation.md) at nonzero [temperature](../../../../temperature-split.md).

For completeness, putting $s=d/\alpha>1$ and using the [Gamma function](../../../../gamma-function.md) and [Riemann zeta function](../../../../riemann-zeta-function.md) gives

$$
n_{\mathrm{ex}}^{\max}(T)=\frac{S_{d-1}}{(2\pi)^d\alpha}c^{-s}\Gamma(s)\zeta(s)(k_BT)^s.
$$

At fixed density $n$, the right-hand side reaches $n$ at $T_c$; below it the excess particles occupy the lowest state, with [condensate fraction](../../../../condensate-fraction.md) $1-(T/T_c)^s$. This is [Bose condensation with power-law dispersion](../../../../bose-condensation-with-power-law-dispersion.md) in the homogeneous [thermodynamic limit](../../../../thermodynamic-limit.md). A finite vessel or a trapping potential changes the low-energy state count and must not be silently substituted for that setting.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
