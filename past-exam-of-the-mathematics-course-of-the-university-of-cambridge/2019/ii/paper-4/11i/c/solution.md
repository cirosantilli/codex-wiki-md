<h1 id="11i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [continued-fraction matrix](../../../../../../continued-fraction-matrix.md) for the original finite continued fraction is

$$
M(a_0)\cdots M(a_n)
=\begin{pmatrix}p_n&p_{n-1}\\q_n&q_{n-1}\end{pmatrix}.
$$

Each $M(a_j)$ is a [symmetric matrix](../../../../../../symmetric-matrix.md), so reversing the order gives the transpose:

$$
M(a_n)\cdots M(a_0)
=\begin{pmatrix}p_n&q_n\\p_{n-1}&q_{n-1}\end{pmatrix}.
$$

Reading off the columns proves the [reversal identity for a finite continued fraction](../../../../../../reversal-identity-for-a-finite-continued-fraction.md):

$$
\boxed{[a_n,\ldots,a_0]=\frac{p_n}{p_{n-1}},
\qquad
[a_n,\ldots,a_1]=\frac{q_n}{q_{n-1}}.}
$$

These are respectively the $n$th and $(n-1)$th convergents of the reversed continued fraction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11I](../../11i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
