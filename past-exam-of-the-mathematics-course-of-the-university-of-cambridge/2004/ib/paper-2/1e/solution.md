<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

Let $L_{ik}=1$ when $k\leq i$ and $L_{ik}=0$ otherwise. The [matrix product](../../../../../matrix-product.md) has entries

$$
(LL^T)_{ij}=\sum_{k=1}^n L_{ik}L_{jk}=\min(i,j),
$$

so $A_n=LL^T$. Both $L$ and its [matrix transpose](../../../../../transpose.md) are [triangular matrices](../../../../../triangular-matrix.md) with diagonal entries one. Multiplicativity of the [determinant](../../../../../determinant.md) therefore gives **$\det A_n=(\det L)^2=1$ for every $n\geq1$**. This [determinant of the minimum-index matrix](../../../../../determinant-of-the-minimum-index-matrix.md) also follows by subtracting each preceding row from the next, working from the bottom upwards: the resulting [matrix](../../../../../matrix.md) is upper triangular with unit diagonal.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
