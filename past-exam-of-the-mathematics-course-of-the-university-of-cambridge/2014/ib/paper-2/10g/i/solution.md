<h1 id="10g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the [determinant](../../../../../../determinant.md) expansion of the [block upper triangular matrix](../../../../../../block-upper-triangular-matrix.md), a nonzero product must assign each of the bottom $n$ rows to one of the last $n$ columns, because the lower-left block is zero. Those rows therefore occupy all the last $n$ columns, leaving the first $n$ columns for the top rows. The contributing permutations are precisely independent permutations within the two blocks. Their signs multiply, so the sum factors:

$$
\boxed{\det\begin{pmatrix}A&C\\0&B\end{pmatrix}=\det A\,\det B.}
$$

The off-diagonal block contributes to no surviving term.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10G](../../10g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
