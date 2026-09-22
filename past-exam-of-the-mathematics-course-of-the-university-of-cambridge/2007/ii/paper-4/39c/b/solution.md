<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two independent columns of $V$ remain independent after multiplication by invertible $S$. Since $R=SV$ has zeros below the second row, its leading two-by-two triangular block is invertible. Hence the image under $S$ of the [invariant subspace](../../../../../../invariant-subspace.md) is exactly $\operatorname{span}(e_1,e_2)$. This coordinate plane is invariant under $\widehat A=SAS^{-1}$, forcing the bottom-left block to vanish:

$$
\widehat A=\begin{pmatrix}B&C\\0&D\end{pmatrix}.
$$

The block determinant factors $\det(zI-\widehat A)=\det(zI-B)\det(zI-D)$. Therefore **the [eigenvalues](../../../../../../eigenvalue.md) of $A$ are exactly those of the indicated two-by-two and $(n-2)$-by-$(n-2)$ blocks**, counted with algebraic multiplicity. No diagonalizability assumption is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
