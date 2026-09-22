<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The two [adjoints of inverse image on power sets](../../../../../../adjoints-of-inverse-image-on-power-sets.md) are

$$
\boxed{\exists_p(U)=p(U),\qquad\forall_p(U)=\{b\in B:p^{-1}(\{b\})\subseteq U\}.}
$$

These maps and $p^*(V)=p^{-1}(V)$ are [monotone functions](../../../../../../monotonic-function.md) on the inclusion-ordered [power sets](../../../../../../power-set.md). For $U\subseteq A$ and $V\subseteq B$,

$$
p(U)\subseteq V\iff U\subseteq p^{-1}(V),\qquad p^{-1}(V)\subseteq U\iff V\subseteq\forall_p(U).
$$

The first equivalence follows by following each element of $U$ through $p$. For the second, every [fiber](../../../../../../fiber-of-a-function.md) over $b\in V$ must lie in $U$, which is precisely the defining condition for $b\in\forall_p(U)$. These are the two [Galois connections](../../../../../../galois-connection.md), proving $\exists_p\dashv p^*\dashv\forall_p$. In particular, a point outside $p(A)$ has an empty [fiber](../../../../../../fiber-of-a-function.md) and belongs to $\forall_p(U)$ even when $U$ is empty; omitting this case would give an incorrect [right adjoint](../../../../../../adjoint-functors.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
