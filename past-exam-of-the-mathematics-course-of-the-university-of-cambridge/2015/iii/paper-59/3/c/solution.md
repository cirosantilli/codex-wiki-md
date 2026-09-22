<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [incompressible planetary interior](../../../../../../incompressible-planetary-interior.md) of density $\rho$, the enclosed mass and local gravity are $M(r)=4\pi\rho r^3/3$ and $g(r)=4\pi G\rho r/3$. [Hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) therefore gives

$$
\frac{dP}{dr}=-\frac{GM(r)\rho}{r^2}=-\frac{4\pi G\rho^2}{3}r.
$$

Integrating inward from negligible surface pressure at $r=R_p$ yields the [uniform-density planetary pressure profile](../../../../../../uniform-density-planetary-pressure-profile.md):

$$
\boxed{P(r)=\frac{2\pi G\rho^2}{3}(R_p^2-r^2)=P_c\left(1-\frac{r^2}{R_p^2}\right),\qquad P_c=\frac{2\pi G\rho^2R_p^2}{3}.}
$$

The surface gravity is $g_s=GM/R_p^2=4\pi G\rho R_p/3$. Eliminate $\rho R_p$ to obtain

$$
\boxed{P_c=\frac{3g_s^2}{8\pi G}.}
$$

The units of $g_s^2/G$ are pressure. For a nonzero imposed surface pressure, add $P_s$ throughout and interpret the boxed central value as $P_c-P_s$. The constant-density approximation is crucial; real centrally concentrated rocky planets need a different profile and generally a larger central pressure at the same mass and radius.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
