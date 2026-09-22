<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

Let $M(r)$ be the [enclosed mass](../../../../../enclosed-mass.md). A spherical shell of thickness $dr$ has inward gravitational acceleration $GM(r)/r^2$, so [hydrostatic equilibrium](../../../../../hydrostatic-pressure-support-equation.md) requires

$$
\boxed{\frac{dP}{dr}=-\frac{GM(r)\rho(r)}{r^2},
\qquad
\frac{dM}{dr}=4\pi r^2\rho(r).}
$$

With $\rho=Ar^2P$, these equations reduce to

$$
P'=-GAMP,
\qquad
M'=4\pi Ar^4P.
$$

For a regular central value $P(0)=P_c>0$, the first equation integrates to

$$
P(r)=P_c\exp\left(-GA\int_0^rM(s)\,ds\right).
$$

The [exponential function](../../../../../exponential-function.md) is strictly positive at every finite $r$, so the pressure and density cannot reach zero at a finite stellar surface. The equations may describe an atmosphere whose density decreases at large radius, but they admit no nontrivial hydrostatic star of finite radius. Therefore

$$
\boxed{\text{there is no stable finite-radius stellar solution with this relation.}}
$$

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
