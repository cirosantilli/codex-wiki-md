<h1 id="12b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $h=u-\phi-C$. Then $h=0$ on $S$, and the constant does not change a [gradient](../../../../../../gradient.md), so $\nabla u=\nabla\phi+\nabla h$. Expand the unnormalized [Dirichlet energy](../../../../../../dirichlet-energy.md):

$$
\int_V|\nabla u|^2\,dV
=\int_V|\nabla\phi|^2\,dV
+2\int_V\nabla\phi\cdot\nabla h\,dV
+\int_V|\nabla h|^2\,dV.
$$

The cross term is zero by [Green's first identity](../../../../../../green-s-first-identity.md):

$$
\int_V\nabla\phi\cdot\nabla h\,dV
=\int_Sh\,\partial_n\phi\,dS-\int_Vh\Delta\phi\,dV=0.
$$

Thus the useful stronger identity is

$$
\boxed{\int_V|\nabla u|^2\,dV-\int_V|\nabla\phi|^2\,dV
=\int_V|\nabla(u-\phi-C)|^2\,dV\geq0.}
$$

Equality holds exactly when $h$ has zero [gradient](../../../../../../gradient.md). It is then constant on every [connected component](../../../../../../connected-component.md) and zero on that component’s boundary, hence $h=0$. Therefore **equality holds precisely when $u=\phi+C$ throughout $V$.** This is the [Dirichlet principle](../../../../../../dirichlet-principle.md); an additive boundary constant does not alter the minimizing energy. The energy here omits the optional factor $1/2$, which does not affect minimizers or the inequality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
