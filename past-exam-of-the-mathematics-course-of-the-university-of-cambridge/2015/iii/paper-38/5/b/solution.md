<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The preceding [perfect matching](../../../../../../perfect-matching.md) gives a [permutation matrix](../../../../../../permutation-matrix.md) $P$ supported on the positive entries of $A$. Let

$$
\alpha=\min\{a_{ij}:p_{ij}=1\}>0.
$$

If $\alpha=1$, every row's selected entry is one and all other entries vanish, so $A=P$. Otherwise

$$
A'=\frac{A-\alpha P}{1-\alpha}
$$

is a [doubly stochastic matrix](../../../../../../doubly-stochastic-matrix.md) with strictly fewer positive entries. Induct on the number of positive entries: the base case has exactly $n$ positive entries and is a [permutation matrix](../../../../../../permutation-matrix.md). By induction, write $A'=\sum_i\beta_iP_i$ as a [convex combination](../../../../../../convex-combination.md). Then

$$
A=\alpha P+(1-\alpha)\sum_i\beta_iP_i
$$

is another [convex combination](../../../../../../convex-combination.md), with nonnegative coefficients summing to one. Thus

$$
\boxed{A=\sum_{i=1}^k\alpha_iP_i,\qquad \alpha_i\geq0,\quad\sum_i\alpha_i=1.}
$$

This constructive proof of the [Birkhoff-von Neumann theorem](../../../../../../birkhoff-von-neumann-theorem.md) is [Birkhoff decomposition by support matchings](../../../../../../birkhoff-decomposition-by-support-matchings.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
