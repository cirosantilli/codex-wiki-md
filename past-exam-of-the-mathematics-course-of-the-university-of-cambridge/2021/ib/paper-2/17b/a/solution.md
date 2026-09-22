<h1 id="17b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero vector $v\in\mathbb R^n$, a [Householder reflection](../../../../../../householder-transformation.md) is

$$
H=I-2\frac{vv^T}{v^Tv}.
$$

It is immediately [symmetric](../../../../../../symmetric-matrix.md). If $P=vv^T/(v^Tv)$, then $P^2=P$, so

$$
H^TH=H^2=(I-2P)^2=I.
$$

Hence $H$ is also an [orthogonal matrix](../../../../../../orthogonal-matrix.md), with $H^{-1}=H$.

The [similarity transformation](../../../../../../similarity-transformation.md) can be expanded as

$$
HAH
=A-2P A-2A P+4PAP.
$$

Computing $v^TA$, $Av$, and the scalar $v^TAv$ costs $O(n^2)$ [arithmetic operations](../../../../../../arithmetic-operation.md), after which the remaining updates are [outer products](../../../../../../outer-product.md) and scalar multiples, also costing $O(n^2)$. Thus $HAH^{-1}$ can be formed in $O(n^2)$ operations rather than by two general $O(n^3)$ [matrix multiplications](../../../../../../matrix-multiplication.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17B](../../17b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
