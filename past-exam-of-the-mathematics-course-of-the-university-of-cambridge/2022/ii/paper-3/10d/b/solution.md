<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the restricted operations, begin in $|0\rangle|0\rangle$ and apply $F$ to the first register:

$$
\frac1{\sqrt N}\sum_i|i\rangle|0\rangle.
$$

Now apply

$$
O_x,\qquad Z,\qquad O_x.
$$

For every basis state this [compute-phase-uncompute construction](../../../../../../compute-phase-uncompute-construction.md) acts as

$$
|i\rangle|0\rangle
\mapsto |i\rangle|x_i\rangle
\mapsto(-1)^{x_i}|i\rangle|x_i\rangle
\mapsto(-1)^{x_i}|i\rangle|0\rangle.
$$

The first register is therefore the same phase state used in part (a). Apply $F^{-1}$ and measure. Again, outcome $0$ occurs with probability one for a constant string and probability zero for a balanced string. The construction uses exactly two queries to $O_x$ and only the permitted operations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
