<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [orthogonality](../../../../../orthogonal-vectors.md) and the sampling property of the [Dirac delta distribution](../../../../../dirac-delta-function.md),

$$
a_n=\rho_0\int_0^L\delta(x-x_0)\psi_n(x)\,dx=\boxed{\rho_0\sqrt{\frac2L}\sin\frac{n\pi x_0}{L}}.
$$

Consequently the [reaction-diffusion equation](../../../../../reaction-diffusion-system.md) solution is

$$
\boxed{\rho(x,t)=\frac{2\rho_0}{L}\sum_{n=1}^{\infty}\sin\frac{n\pi x_0}{L}\sin\frac{n\pi x}{L}\exp\left[\left(\gamma-\frac{Dn^2\pi^2}{L^2}\right)t\right].}
$$

For every $t>0$ this [eigenfunction expansion](../../../../../eigenfunction-expansion.md) is smoothed by the Gaussian decay in $n$. As $t\downarrow0$, it recovers the specified initial condition in the sense of [distributions](../../../../../distribution-mathematical-analysis.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
