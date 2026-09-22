<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a row of descending monomials $T(t)=[t^2\ t\ 1]$ and a [matrix](../../../../../matrix.md) with one [control point](../../../../../control-point.md) per row. Expanding $(1-t)^2,2t(1-t),t^2$ gives their [coefficients](../../../../../coefficient.md) in the three columns of the basis [matrix](../../../../../matrix.md):

$$
M_B=\begin{pmatrix}1&-2&1\\-2&2&0\\1&0&0\end{pmatrix},\qquad
G_B=\begin{pmatrix}-2&0\\0&1\\0&0\end{pmatrix}.
$$

The [matrix multiplication](../../../../../matrix-multiplication.md) is

$$
\boxed{F(t)=T(t)M_BG_B
=[t^2\ t\ 1]\begin{pmatrix}-2&-2\\4&2\\-2&0\end{pmatrix}.}
$$

In particular, $T(t)M_B=[(1-t)^2\ 2t(1-t)\ t^2]$, so multiplying the geometric [matrix](../../../../../matrix.md) takes exactly the weighted [control point](../../../../../control-point.md) sum in part (a). The two output entries are $F_x(t),F_y(t)$. The basis [matrix](../../../../../matrix.md) depends only on the degree and ordering convention; $G_B$ holds the particular geometry.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
