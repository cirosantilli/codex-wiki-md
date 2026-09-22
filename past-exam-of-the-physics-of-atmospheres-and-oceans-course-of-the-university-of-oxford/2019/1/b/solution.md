<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the requested [mass path](../../../../mass-path.md) as the vapour column; no condensed-water loading is prescribed. [Hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) gives $dp=-\rho g\,dz$, so if $q_B=\rho_B/\rho$ is vapour [mass fraction](../../../../mass-fraction.md),

$$
W_B=\int_0^\infty\rho_B\,dz=\frac1g\int_0^{p_s}q_B(p)\,dp.
$$

For the mixture $q_B=\epsilon e_s/[p+(\epsilon-1)e_s]$. Under the dilute conditions of part (a), $q_B\simeq\epsilon e_s/p$. Introduce $\zeta=-\ln(p/p_s)$, so $T=T_se^{-x\zeta}$ and $-dp=p\,d\zeta$. Integrating the constant-$L$ [Clausius-Clapeyron equation](../../../../clausius-clapeyron-relation.md) relative to the surface gives

$$
e_s(T)=e_s(T_s)\exp\left[-\frac{L}{R_B}\left(\frac1T-\frac1{T_s}\right)\right].
$$

Therefore

$$
\boxed{W_B\simeq\frac{\epsilon e_s(T_s)}g\int_0^\infty\exp[-\beta_s(e^{x\zeta}-1)]\,d\zeta,\qquad \beta_s=\frac{L}{R_BT_s}.}
$$

The explicit $p_s$ cancels: decreasing vapour [mass fraction](../../../../mass-fraction.md) in a denser dry column compensates its greater total [mass](../../../../mass.md). This cancellation belongs to the dilute, dry-adiabatic approximation, and is not a general property of moist atmospheres. With suspended condensate, an additional and unspecified condensate [mass path](../../../../mass-path.md) would have to be added.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
