<h1 id="10h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [matrix trace](../../../../../../matrix-trace.md) is the sum of diagonal entries, $\operatorname{tr}A=\sum_{i=1}^nA_{ii}$. For any two square [matrices](../../../../../../matrix.md),

$$
\operatorname{tr}(BC)=\sum_{i,j}B_{ij}C_{ji}
=\sum_{j,i}C_{ji}B_{ij}=\operatorname{tr}(CB).
$$

Apply this [cyclic property of the trace](../../../../../../cyclic-property-of-the-trace.md) with $B=T$ and $C=AT^{-1}$:

$$
\boxed{\operatorname{tr}(TAT^{-1})=\operatorname{tr}(AT^{-1}T)=\operatorname{tr}A.}
$$

Thus [matrix similarity](../../../../../../matrix-similarity.md) preserves the [matrix trace](../../../../../../matrix-trace.md); no assumption that either [matrix](../../../../../../matrix.md) is diagonalizable is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10H](../../10h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
