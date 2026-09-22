<h1 id="18/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Subtracting the second row from the third gives a third row $(0,2,0)$, so expansion along it shows $\det B=-2\ne0$. Thus the [matrix inverse](../../../../../../matrix-inverse-split.md) exists and every right-hand side has a unique solution.

To calculate it, temporarily solve $B\mathbf x=\mathbf b$ with general $\mathbf b=(b_1,b_2,b_3)^T$. Subtracting the second equation from the third and from the first gives

$$
2x_2=b_3-b_2,\qquad x_1-x_2=b_1-b_2.
$$

Back-substitution into the second equation gives

$$
x_1=b_1-\frac32b_2+\frac12b_3,\quad x_2=-\frac12b_2+\frac12b_3,\quad x_3=-b_1+\frac72b_2-\frac32b_3.
$$

Therefore

$$
\boxed{B^{-1}=\begin{pmatrix}1&-3/2&1/2\\0&-1/2&1/2\\-1&7/2&-3/2\end{pmatrix}.}
$$

For the given right-hand side, [matrix multiplication](../../../../../../matrix-multiplication.md) yields the unique answer

$$
\boxed{\mathbf x=B^{-1}(1,2,3)^T=(-1/2,1/2,3/2)^T.}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [18](../../../18.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
