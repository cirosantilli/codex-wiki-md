<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho:\pi_1(X)\to U(V)$ be the [unitary representation](../../../../../../unitary-representation.md). The associated [unitary flat holomorphic vector bundle](../../../../../../unitary-flat-holomorphic-vector-bundle.md) is

$$
E_V=(\widetilde X\times V)/\pi_1(X),
$$

where deck transformations act on the first factor and $\rho$ acts on the second. Local lifts to the [universal cover](../../../../../../universal-cover.md) give holomorphic orthonormal frames with locally constant unitary transition matrices. The induced [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) is therefore well defined, and the induced flat [unitary connection](../../../../../../unitary-connection.md) is its [Chern connection](../../../../../../chern-connection.md).

Let $s$ be a global [holomorphic section](../../../../../../holomorphic-section.md). In one of these parallel orthonormal frames write $s=(f_1,\ldots,f_r)$, where every $f_j$ is holomorphic. Its squared norm $u=|s|^2=\sum_j|f_j|^2$ is a globally defined smooth function because the transition matrices are unitary. In a local complex coordinate,

$$
\frac{\partial^2u}{\partial z\,\partial\bar z}=\sum_{j=1}^r|f'_j(z)|^2\ge0.
$$

Choose any smooth conformal metric on the curve, locally $\kappa(z)|dz|^2$. Its Laplacian satisfies

$$
\Delta u=\frac4\kappa\sum_j|f'_j|^2\ge0.
$$

On the compact curve without boundary, [Stokes theorem](../../../../../../stokes-theorem.md) gives $\int_X\Delta u\,d\mathrm{vol}=0$. A continuous nonnegative function with zero integral vanishes everywhere, so each $f'_j=0$. Thus the section is locally constant in every parallel frame and is globally parallel. This proves that [holomorphic sections of a unitary flat bundle are parallel](../../../../../../holomorphic-sections-of-a-unitary-flat-bundle-are-parallel.md).

A parallel section is determined by its value $v$ at a chosen base point. Following it around a loop returns the value $\rho(\gamma)v$, so a global parallel section exists exactly when $\rho(\gamma)v=v$ for every $\gamma\in\pi_1(X)$. Conversely, such a fixed vector gives the constant equivariant section on $\widetilde X$, which descends holomorphically. Evaluation and this construction are inverse linear maps, giving the canonical identification

$$
\boxed{H^0(X,E_V)\cong V^{\pi_1(X)}.}
$$

Unitarity is what makes the local squared norms glue and the integrated nonnegative identity available; no assumption that the universal cover is compact is made.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
