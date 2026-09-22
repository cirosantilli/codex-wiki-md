<h1 id="3/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Let $v=\operatorname{prox}_J(u)$ and $p=u-v$. The [proximal operator](../../../../../../proximal-operator.md) optimality condition gives $p\in\partial J(v)$. By [subgradient inversion under convex conjugacy](../../../../../../subgradient-inversion-under-convex-conjugacy.md), $v\in\partial J^*(p)$. Since $v=u-p$, this is exactly the optimality condition defining $p=\operatorname{prox}_{J^*}(u)$. Uniqueness of both Hilbert proximal minimizers proves [Moreau decomposition](../../../../../../moreau-decomposition.md):

$$
\boxed{u=\operatorname{prox}_J(u)+\operatorname{prox}_{J^*}(u).}
$$

Both terms belong to the same [Hilbert space](../../../../../../hilbert-space-split.md) after dual identification. No orthogonality of the two terms is asserted for a general convex $J$; that stronger property pertains to special indicator/cone cases.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
