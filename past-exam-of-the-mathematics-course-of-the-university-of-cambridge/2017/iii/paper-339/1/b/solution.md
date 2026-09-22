<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x$ in the [nonnegative orthant](../../../../../../nonnegative-orthant.md), the [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) $P$ satisfies $x^TPx\geq0$. The [nonnegative matrix](../../../../../../nonnegative-matrix.md) $N$ satisfies

$$
x^TNx=\sum_{i,j}N_{ij}x_ix_j\geq0,
$$

since every summand is nonnegative. Adding these inequalities proves

$$
\boxed{x^T(P+N)x\geq0\quad(x\geq0)}.
$$

Consequently $A=P+N$ is a [copositive matrix](../../../../../../copositive-matrix.md). The symmetry of $N$ follows from that of $A$ and $P$; entrywise nonnegativity alone need not imply [positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md).

This gives the inclusion of the [positive-semidefinite-plus-nonnegative cone](../../../../../../positive-semidefinite-plus-nonnegative-cone.md) in the [copositive cone](../../../../../../copositive-cone.md). It is only a sufficient construction; the argument does not claim that every [copositive matrix](../../../../../../copositive-matrix.md) has this decomposition in arbitrary [dimension](../../../../../../dimension-vector-space.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
