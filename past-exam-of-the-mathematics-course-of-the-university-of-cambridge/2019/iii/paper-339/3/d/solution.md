<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $w=(1,2,1,0,0)^T$. Direct multiplication gives $Hw=(0,0,0,2,2)^T$, so $w^THw=0$.

Suppose $H=P+N$, where $P$ is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) and $N$ is a symmetric [nonnegative matrix](../../../../../../nonnegative-matrix.md). Since $w\geq0$, both $w^TPw$ and $w^TNw$ are nonnegative. Their sum is zero, so both vanish. In particular,

$$
0=w^TNw=\sum_{i,j=1}^3 w_iw_jN_{ij}.
$$

Every coefficient $w_iw_j$ in this sum is strictly positive and every $N_{ij}$ is nonnegative, forcing $N_{ij}=0$ for $1\leq i,j\leq3$.

Now apply the same argument to all five cyclic shifts of $w$. The [Horn copositive matrix](../../../../../../horn-copositive-matrix.md) is cyclically invariant, so every shifted [vector](../../../../../../vector.md) also has zero [quadratic form](../../../../../../quadratic-form.md). It follows that the entries of $N$ vanish on every cyclic block of three consecutive indices. Every pair of indices on a five-cycle lies in such a block, hence $N=0$.

This would imply $P=H$. But the [zero quadratic form of a positive semidefinite matrix](../../../../../../zero-quadratic-form-of-a-positive-semidefinite-matrix.md) would then force $Hw=0$, contradicting $Hw=(0,0,0,2,2)^T$. Therefore $H$ lies outside the [positive-semidefinite-plus-nonnegative cone](../../../../../../positive-semidefinite-plus-nonnegative-cone.md). By the previous equivalence, its quartic form is a [nonnegative polynomial](../../../../../../nonnegative-polynomial.md) that is not a [sum of squares polynomial](../../../../../../polynomial-sos.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
