<h1 id="19g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For any [idempotent linear map](../../../../../../projection-linear-algebra.md) $\tau$, each vector decomposes as

$$
u=(u-\tau u)+\tau u,\qquad \tau(u-\tau u)=0,\qquad\tau u\in\operatorname{im}\tau.
$$

If $w\in\ker\tau\cap\operatorname{im}\tau$, write $w=\tau v$; then $0=\tau w=\tau^2v=\tau v=w$. Thus the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) and [image of a linear map](../../../../../../image-of-a-linear-map.md) give a [direct sum](../../../../../../direct-sum.md).

For the self-adjoint map in the question, $k\in\ker\tau$ and $w=\tau v$ satisfy $\langle k,w\rangle=\langle k,\tau v\rangle=\langle\tau k,v\rangle=0$. Hence the direct sum is an [orthogonal decomposition](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md):

$$
\boxed{U=\ker\tau\mathbin\oplus^{\perp}\operatorname{im}\tau.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19G](../../19g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
