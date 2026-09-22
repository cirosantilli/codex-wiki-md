<h1 id="12c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For two solutions of the [Poisson equation](../../../../../../poisson-equation.md) with the same [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md), let $w=u_1-u_2$. Then $\nabla^2w=0$ in $V$ and $w=0$ on its boundary. By [Green's first identity](../../../../../../green-s-first-identity.md),

$$
\int_V|\nabla w|^2\,dV
=\int_Sw\,\partial_nw\,dS-\int_Vw\nabla^2w\,dV=0.
$$

Thus $w$ is constant on each connected component, and the zero boundary values make each constant zero. **The Dirichlet solution is unique whenever it exists.** This argument requires the regularity needed for the displayed integration by parts; it does not assert existence for arbitrary rough data.

With a [Neumann boundary condition](../../../../../../neumann-boundary-condition.md), integrating the [Poisson equation](../../../../../../poisson-equation.md) and using the [divergence theorem](../../../../../../divergence-theorem.md) instead gives the necessary compatibility condition

$$
\boxed{\int_V\rho\,dV=\int_Sg\,dS.}
$$

On a disconnected region this condition must hold on each connected component separately. If two solutions have the same normal derivative, their difference is harmonic with $\partial_nw=0$. The same [Green's first identity](../../../../../../green-s-first-identity.md) again forces $\nabla w=0$. Thus **Neumann solutions are unique only up to an additive constant on each connected component**. Adding a constant preserves both the equation and normal derivative, so uniqueness without a normalization cannot hold. On a connected region, prescribing the mean value removes this one-dimensional freedom.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12C](../../12c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
