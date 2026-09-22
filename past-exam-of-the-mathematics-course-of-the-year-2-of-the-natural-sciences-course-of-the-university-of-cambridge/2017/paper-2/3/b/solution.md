<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is the [Dirichlet principle](../../../../../dirichlet-principle.md). Put $v=w-\psi$, so $v$ vanishes on the boundary. For real, sufficiently regular functions of finite [Dirichlet energy](../../../../../dirichlet-energy.md), [Green's first identity](../../../../../green-s-first-identity.md) gives

$$
\int_V\nabla\psi\cdot\nabla v\,dV=\int_Sv\,\partial_n\psi\,dS-\int_Vv\nabla^2\psi\,dV=0.
$$

The surface term is zero because $v=0$, and the volume term is zero because $\psi$ is a [harmonic function](../../../../../harmonic-function.md). Expanding the square of $\nabla w=\nabla\psi+\nabla v$ now gives the stronger identity

$$
\boxed{\int_V|\nabla w|^2\,dV=\int_V|\nabla\psi|^2\,dV+\int_V|\nabla(w-\psi)|^2\,dV\ \geq\ \int_V|\nabla\psi|^2\,dV.}
$$

Thus the [harmonic function](../../../../../harmonic-function.md) minimizes [Dirichlet energy](../../../../../dirichlet-energy.md) among functions with the same boundary values. Equality requires $\nabla v=0$, hence $v$ is constant on each connected component; the zero boundary value makes that constant zero on every component having boundary. For an unbounded domain one additionally needs the boundary term at infinity to vanish; the usual bounded regular-domain setting needs no such extra condition.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
