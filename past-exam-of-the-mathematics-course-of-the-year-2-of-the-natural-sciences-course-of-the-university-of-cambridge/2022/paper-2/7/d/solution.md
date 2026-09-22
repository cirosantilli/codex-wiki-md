<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The pinned third bar has zero displacement, so remove its row and column from the [stiffness matrix](../../../../../stiffness-matrix.md) while retaining the [springs](../../../../../spring.md) that connect the moving bars to it. The remaining unit-mass system has

$$
K_{\rm pin}=k\begin{pmatrix}3&-1\\-1&3\end{pmatrix}.
$$

Its [eigenvectors](../../../../../eigenvector.md) $(1,1)^T$ and $(1,-1)^T$ have [eigenvalues](../../../../../eigenvalue.md) $2k$ and $4k$. Hence

$$
\boxed{\omega_{\rm in\ phase}=\sqrt{2k},\qquad\omega_{\rm out\ of\ phase}=2\sqrt{k}.}
$$

For $k=1$ these are $\sqrt2$ and $2$. The fixed value $X_3=0$ changes the static offsets and reaction force but not this linearized [matrix](../../../../../matrix.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
