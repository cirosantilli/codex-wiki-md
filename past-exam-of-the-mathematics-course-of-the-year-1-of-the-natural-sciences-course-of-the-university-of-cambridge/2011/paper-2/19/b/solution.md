<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D=(1-x)^2+y^2$. Direct [partial differentiation](../../../../../partial-derivative.md), away from $(1,0)$, gives

$$
u_x=v_y=\frac{2((1-x)^2-y^2)}{D^2},\qquad
u_y=-v_x=-\frac{4(1-x)y}{D^2}.
$$

These are the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). Equivalently, with $z=x+iy$, the analytic mapping is $u+iv=(1+z)/(1-z)$, the inverse [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md).

The supplied harmonicity result can also be checked by the [multivariable chain rule](../../../../../multivariable-chain-rule.md). The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) imply $\Delta u=\Delta v=0$, $\nabla u\cdot\nabla v=0$, and $|\nabla u|^2=|\nabla v|^2$. Hence

$$
\Delta\Psi=(u_x^2+u_y^2)(\Phi_{uu}+\Phi_{vv})=0.
$$

This is [conformal invariance of harmonicity](../../../../../conformal-invariance-of-harmonicity.md) for the given mapping.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
