<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume a positive common density scale $\rho_0$ and use the unit-radius coordinates of the source. The cylinder's density depends on distance from its axis. Its [mass](../../../../mass.md) is

$$
M_{\mathrm{cyl}}=\int_0^4\int_0^{2\pi}\int_0^1\rho_0r^{-1}\,r\,dr\,d\phi\,dz
=8\pi\rho_0.
$$

The radial factor in the [cylindrical volume element](../../../../cylindrical-volume-element.md) cancels the apparent density singularity.

For the sphere, the [spherical volume element](../../../../spherical-volume-element.md) gives

$$
M_{\mathrm{sph}}=4\pi\rho_0\int_0^1r^{n+2}\,dr
=\frac{4\pi\rho_0}{n+3},\qquad n>-3.
$$

The condition is necessary for finite [mass](../../../../mass.md); the integral diverges for $n\leq-3$. Equating the two finite masses yields $1/(n+3)=2$, and hence

$$
\boxed{n=-\frac52.}
$$

This satisfies $n>-3$. A divergent pointwise density can therefore have finite total [mass](../../../../mass.md): the [integrable power-law density at an axis or center](../../../../integrable-power-law-density-at-an-axis-or-center.md) must be tested together with its volume factor. Dimensionally, the density laws can be understood as $\rho_0(r/R)^{-1}$ and $\rho_0(r/R)^n$ with unit radius $R=1$ in the chosen length units.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
