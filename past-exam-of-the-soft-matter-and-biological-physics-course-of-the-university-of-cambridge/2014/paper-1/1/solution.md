<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[velocity](../../../../velocity.md) $U$, [length](../../../../length.md) $\ell$ and [diffusivity](../../../../diffusion-coefficient.md) $D$ have dimensions $L/T$, $L$, and $L^2/T$. Their dimensionless [Péclet number](../../../../peclet-number.md) is

$$
\boxed{\mathrm{Pe}=\frac{U\ell}{D}=\frac{\ell^2/D}{\ell/U}.}
$$

[diffusion](../../../../diffusion.md) dominates for $\mathrm{Pe}\ll1$, [advection](../../../../advection.md) for $\mathrm{Pe}\gg1$. At fixed $U,D$, the crossover [length](../../../../length.md) is $D/U$; neglecting [advection](../../../../advection.md) requires $\ell\ll D/U$.

TODO: user-deferred organism-specific swimming-speed and detection-scale estimates. No biological numerical substitution is made.

For the generic [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) transport derivation, let an external potential $V(x)$ give [force](../../../../force-split.md) $F=-V'$ and drift $u=F/\zeta$. Boltzmann [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) has $c\propto e^{-V/(k_BT)}$, hence $c'=Fc/(k_BT)$. Substituting in the zero-current condition gives

$$
J=Fc\left(\frac1\zeta-\frac{D}{k_BT}\right)=0,
\qquad\boxed{D=\frac{k_BT}{\zeta}=\frac{k_BT}{6\pi\eta a}.}
$$

The [Stokes–Einstein relation](../../../../stokes-einstein-relation.md) in the final equality is for an isolated no-slip sphere in a Newtonian liquid at low [Reynolds number](../../../../reynolds-number.md). Zero flux alone is insufficient: the [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) distribution and mechanical mobility law are also needed.

TODO: user-deferred organism-specific absorbing-surface calculation and its biological flux interpretation.

TODO: user-deferred receptor-number, receptor-density and receptor-competition calculations. These continuations have not been solved.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the soft matter and biological physics course of the University of Cambridge](../../../split.md)
5. [Soft Matter and Biological Physics course of the University of Cambridge](../../../../soft-matter-and-biological-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
