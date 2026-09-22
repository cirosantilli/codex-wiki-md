<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For ordinary condensibles, $L/(R_BT)$ is typically of order ten or more near low atmospheric temperatures. At the approximate triple-point [temperatures](../../../../temperature-split.md), the supplied substances give $\beta$ about $20$ for water and $10$–$12$ for carbon dioxide, methane and nitrogen. This is consistent with the supplied large ratios of [latent heat](../../../../latent-heat.md) to sensible heating: for molecular gases $c_p/R$ is only a few. The relevant $x=R_A/c_{pA}$ is typically a few tenths.

The [integral](../../../../integral-split.md) is concentrated where $\beta_sx\zeta=O(1)$. There $x\zeta=O(\beta_s^{-1})\ll1$, so $e^{x\zeta}-1\simeq x\zeta$ gives

$$
\boxed{W_B\simeq\frac{\epsilon e_s(T_s)}{g x\beta_s}=\frac{c_{pA}T_s}{L}\frac{e_s(T_s)}g.}
$$

This is an [Laplace's method](../../../../laplace-s-method.md), rather than an assumption that vapour is uniformly mixed. The effective contributing depth in log-pressure is $\Delta\zeta\sim1/(x\beta_s)$, explaining why the near-surface atmosphere dominates.

An exact representation within the same dilute model makes the error explicit. Set $y=\beta_se^{x\zeta}$ and define the [exponential integral](../../../../exponential-integral.md) $E_1(b)=\int_b^\infty e^{-y}dy/y$. Then

$$
W_B=\frac{\epsilon e_s(T_s)}{gx}e^{\beta_s}E_1(\beta_s)
\sim\frac{c_{pA}T_s e_s(T_s)}{gL}\left(1-\frac1{\beta_s}+\frac2{\beta_s^2}-\cdots\right).
$$

The [saturated vapor column on a dry adiabat](../../../../saturated-vapor-column-on-a-dry-adiabat.md) estimate overstates the exact dilute-model column by roughly $1/\beta_s$, about five to ten per cent for those illustrative values. It is not accurate for a warm, nondilute steam atmosphere.

## ↑ Ancestors (12)

1. [C](../c.md)
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
