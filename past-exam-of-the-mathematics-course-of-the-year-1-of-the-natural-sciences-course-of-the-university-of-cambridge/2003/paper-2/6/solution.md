<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use [Gaussian elimination](../../../../gaussian-elimination.md). The last equation gives $y=c-z$, and the second then gives $x=b-4c-2z$. Substitute these into the first equation to obtain $3b-10c-z=a$. Back-substitution yields

$$
\boxed{x=2a-5b+16c,\qquad y=a-3b+11c,\qquad z=-a+3b-10c.}
$$

The [linear system](../../../../system-of-linear-equations.md) has [matrix](../../../../matrix.md) form

$$
\begin{pmatrix}3&2&7\\1&4&6\\0&1&1\end{pmatrix}\begin{pmatrix}x\\y\\z\end{pmatrix}=\begin{pmatrix}a\\b\\c\end{pmatrix}.
$$

The coefficients of the arbitrary right-hand side in the solved expressions are the rows of the [matrix inverse](../../../../matrix-inverse-split.md). Therefore

$$
\boxed{\begin{pmatrix}3&2&7\\1&4&6\\0&1&1\end{pmatrix}^{-1}=\begin{pmatrix}2&-5&16\\1&-3&11\\-1&3&-10\end{pmatrix}.}
$$

Multiplying the original [matrix](../../../../matrix.md) by this candidate gives the [identity matrix](../../../../identity-matrix.md); its [determinant](../../../../determinant.md) is $-1$, so the solution is unique for every $(a,b,c)$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
