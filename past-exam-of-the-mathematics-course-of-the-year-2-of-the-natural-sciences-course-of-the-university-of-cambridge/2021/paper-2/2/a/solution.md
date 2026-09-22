<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $\Psi_1$ and $\Psi_2$ have the same boundary data, and put $u=\Psi_1-\Psi_2$. Then $\Delta u=0$ in $V$ and $u=0$ on its boundary. For real $u$, the [product rule](../../../../../product-rule.md) for the [divergence](../../../../../divergence.md) gives

$$
\nabla\cdot(u\nabla u)=|\nabla u|^2+u\Delta u=|\nabla u|^2.
$$

The [divergence theorem](../../../../../divergence-theorem.md) therefore yields

$$
\int_V|\nabla u|^2dV=\int_Su\,\partial_nu\,dS=0.
$$

The nonnegative integrand must vanish, so $\nabla u=0$ throughout $V$. On each connected component $u$ is constant, and its zero boundary value makes that constant zero. Hence $\boxed{\Psi_1=\Psi_2}$, proving uniqueness. For complex fields, apply the same argument to real and imaginary parts, or use $\nabla\cdot(u^*\nabla u)$ and its real part.

This is [Dirichlet uniqueness for the Poisson equation](../../../../../dirichlet-uniqueness-for-the-poisson-equation.md) applied to the difference of two [harmonic functions](../../../../../harmonic-function.md). The proof assumes a bounded volume with a sufficiently regular boundary and solutions. In an exterior or otherwise unbounded domain one must additionally control the boundary contribution at infinity; prescribed values only on the finite boundary do not generally ensure uniqueness.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
