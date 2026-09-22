<h1 id="9b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $\phi_1,\phi_2$ solve the Dirichlet problem and put $u=\phi_1-\phi_2$. Then $\nabla^2u=0$ in $V$ and $u=0$ on $S$. The [divergence theorem](../../../../../../divergence-theorem.md) applied to $u\nabla u$ gives Green's identity

$$
\int_V|\nabla u|^2\,dV
=\int_Su\,\partial_nu\,dS-
\int_Vu\nabla^2u\,dV=0.
$$

Thus $\nabla u=0$, so $u$ is constant; its zero boundary value makes it zero. The Dirichlet solution is therefore unique.

For homogeneous Neumann data the same calculation again shows that $u$ is constant, but the [boundary condition](../../../../../../boundary-condition.md) does not determine that constant. Hence, whenever a Neumann solution exists, adding any constant produces another solution. This is the standard [uniqueness of Poisson equation](../../../../../../uniqueness-of-poisson-equation.md) distinction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9B](../../9b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
