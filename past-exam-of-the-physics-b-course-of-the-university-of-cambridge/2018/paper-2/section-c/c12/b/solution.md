<h1 id="section-c/c12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a long wire away from its ends, the steady [temperature](../../../../../../temperature-split.md) is independent of axial position and azimuth. The [heat equation](../../../../../../heat-equation.md) reduces to

$$
\frac1\rho\frac{d}{d\rho}\left(\rho\frac{dT}{d\rho}\right)=-\frac{H}{\kappa}.
$$

Multiplying by $\rho$ and integrating gives

$$
\rho T'=-\frac{H\rho^2}{2\kappa}+C_1,
\qquad
T=-\frac{H\rho^2}{4\kappa}+C_1\ln\rho+C_2.
$$

A finite [temperature](../../../../../../temperature-split.md) and nonsingular flux at the axis require $C_1=0$. Applying $T(a)=T_0$ determines $C_2=T_0+Ha^2/(4\kappa)$. Therefore

$$
\boxed{T(\rho)=T_0+\frac{H}{4\kappa}(a^2-\rho^2)
=T_0+\frac{I^2}{4\pi^2a^4\kappa\sigma}(a^2-\rho^2).}
$$

This is the [steady temperature of a uniformly heated cylindrical wire](../../../../../../steady-temperature-of-a-uniformly-heated-cylindrical-wire.md). Its hottest point is at the centre, with $T(0)-T_0=I^2/(4\pi^2a^2\kappa\sigma)$. The outward [heat flux](../../../../../../heat-flux-density.md) is $J_Q(\rho)=-\kappa T'(\rho)=H\rho/2$, so the [power](../../../../../../power.md) crossing a cylindrical surface per unit length, $2\pi\rho J_Q(\rho)=H\pi\rho^2$, equals the heating generated inside it.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C12](../../c12.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
