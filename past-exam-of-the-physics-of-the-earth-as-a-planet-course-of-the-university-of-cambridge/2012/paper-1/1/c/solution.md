<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [flux-driven convective layer cooling](../../../../../flux-driven-convective-layer-cooling.md), use $E=C\theta^{4/3}$ with the same unspecified coefficient as in (b). The steady [heat](../../../../../heat-split.md) balance gives

$$
\boxed{\overline T_*=T_s+\theta_*,\qquad
\theta_*=(F/C)^{3/4}=\left(\frac{F}{k}\right)^{3/4}\left(\frac{R_c\eta\kappa}{\rho_0g\alpha}\right)^{1/4}.}
$$

The corresponding boundary-layer thickness is

$$
\delta_*=\frac{k\theta_*}{F}=\left(\frac{kR_c\eta\kappa}{\rho_0g\alpha F}\right)^{1/4}.
$$

Set $\theta=\theta_*+\epsilon$ and expand the [heat](../../../../../heat-split.md) loss to first order. Since $E'(\theta_*)=(4/3)C\theta_*^{1/3}=4F/(3\theta_*)$,

$$
\frac{kd}{\kappa}\dot\epsilon=-\frac{4F}{3\theta_*}\epsilon,
\qquad
\boxed{\epsilon(t)=\epsilon(0)e^{-t/\tau},\quad
\tau=\frac{3kd\theta_*}{4\kappa F}=\frac{3d\delta_*}{4\kappa}.}
$$

This is the _near-equilibrium_ [relaxation time](../../../../../relaxation-time.md). The full equation is nonlinear, so an arbitrary large initial [temperature](../../../../../temperature-split.md) departure need not decay as one exponential. Positive [heat](../../../../../heat-split.md) loss [derivative](../../../../../derivative.md) makes the [steady state](../../../../../steady-state.md) stable. In particular, $\tau$ scales with $d\delta_*$, rather than $d^2$, because [convection](../../../../../convection-split.md) shortens the effective heat-transport distance to the [boundary layer](../../../../../boundary-layer.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../split.md)
6. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
