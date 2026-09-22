<h1 id="12b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Green's first identity](../../../../../../green-s-first-identity.md) and the boundary condition give

$$
\int_V|\nabla u|^2dV
=\int_Su\frac{\partial u}{\partial n}dS-\int_Vu\nabla^2u\,dV=0.
$$

Thus $\nabla u=0$, so $u$ is constant on each connected component of $V$; its zero boundary value forces $\boxed{u=0}$.

Since $w-v=0$ on $S$ and $\nabla^2v=0$, another application of [Green's first identity](../../../../../../green-s-first-identity.md) gives

$$
\int_V\nabla v\mathbin\cdot\nabla(w-v)dV=0.
$$

Consequently

$$
\boxed{\int_V\nabla v\mathbin\cdot\nabla w\,dV
=\int_V|\nabla v|^2dV}.
$$

Expanding $\nabla w=\nabla v+\nabla(w-v)$ and using the vanishing cross term yields the [Dirichlet principle](../../../../../../dirichlet-principle.md)

$$
\boxed{\int_V|\nabla w|^2dV
=\int_V\left(|\nabla v|^2+|\nabla(w-v)|^2\right)dV
\geq\int_V|\nabla v|^2dV}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
