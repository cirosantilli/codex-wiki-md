<h1 id="18/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Compute the two sides of the [normal equations for linear least squares](../../../../../../normal-equations-for-linear-least-squares.md) and divide by $n$:

$$
\begin{pmatrix}1&\overline x\\\overline x&\overline{x^2}\end{pmatrix}
\begin{pmatrix}\alpha\\\beta\end{pmatrix}
=\begin{pmatrix}\overline y\\\overline{xy}\end{pmatrix}.
$$

The first equation gives $\alpha=\overline y-\beta\overline x$. Substitute this into the second and solve:

$$
\boxed{\beta=\frac{\overline{xy}-\overline x\,\overline y}{\overline{x^2}-\overline x^{\,2}},\qquad
\alpha=\frac{\overline{x^2}\,\overline y-\overline x\,\overline{xy}}{\overline{x^2}-\overline x^{\,2}}.}
$$

These [simple linear regression](../../../../../../simple-linear-regression.md) coefficients are unique provided the observed distances are not all equal, since

$$
\overline{x^2}-\overline x^{\,2}=\frac1n\sum_{i=1}^n(x_i-\overline x)^2>0.
$$

The condition $n\ge2$ alone does not guarantee this. If all $x_i=x_0$, the [design matrix](../../../../../../design-matrix.md) has [matrix rank](../../../../../../matrix-rank.md) one and the valid alternative is the family

$$
\boxed{\alpha+x_0\beta=\overline y,\qquad\beta\text{ arbitrary}.}
$$

In this [rank-deficient ordinary least squares](../../../../../../rank-deficient-ordinary-least-squares.md) case, the fitted predictions are uniquely $\overline y$ but the two parameters cannot be separately determined.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [18](../../../18.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
