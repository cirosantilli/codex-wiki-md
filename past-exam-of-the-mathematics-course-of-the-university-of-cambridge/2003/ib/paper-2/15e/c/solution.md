<h1 id="15e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume for contradiction that $n>m$. Apply part b to the [matrix](../../../../../../matrix.md) of the given relation [coefficients](../../../../../../coefficient.md), whose columns are nonzero. For its first dependent prefix choose $b_1,\ldots,b_k$ with

$$
\sum_{j=1}^ka_{ij}b_j=0\quad\text{for all }i,
\qquad z_i:=\sum_{j=1}^ka_{ij}\lambda_jb_j\text{ not all zero}.
$$

Multiply the $j$th given vector relation by $b_j$ and sum. Interchanging the finite sums gives

$$
0=\sum_{i=1}^m\left(\sum_{j=1}^ka_{ij}b_j\right)v_i
+\sum_{i=1}^m\left(\sum_{j=1}^ka_{ij}\lambda_jb_j\right)w_i
=\sum_{i=1}^mz_iw_i.
$$

The $w_i$ are a [basis](../../../../../../basis.md), so all $z_i$ must be zero, contradicting part b. Therefore **$n\le m$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15E](../../15e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
