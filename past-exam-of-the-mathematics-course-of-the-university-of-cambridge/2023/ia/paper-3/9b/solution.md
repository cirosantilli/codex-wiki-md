<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

Using the product rule for directional [derivatives](../../../../../derivative.md),

$$
\partial_t(u\cdot w)
=(w\cdot\nabla)\left(\frac12|u|^2-P\right)
+(u\cdot\nabla)(-u\cdot w).
$$

Thus $f=|u|^2/2-P$ and $g=-h$. If $\nabla\cdot u=0$ and $w=\nabla\times u$, then $\nabla\cdot w=0$. Integrating the two directional [derivatives](../../../../../derivative.md) as divergences gives only boundary fluxes, which vanish because $u\cdot n=w\cdot n=0$. This is [helicity conservation by tangent boundary conditions](../../../../../helicity-conservation-by-tangent-boundary-conditions.md), so $dH/dt=0$.

For the stated field, direct use of the cylindrical curl gives $u\cdot w=-2a\rho^4\sin^2z$. Therefore

$$
\boxed{H=-2a\int_0^{2\pi}d\phi\int_0^\pi\sin^2z\,dz
\int_0^a\rho^5d\rho
=-\frac{\pi^2a^7}{3}.}
$$

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
