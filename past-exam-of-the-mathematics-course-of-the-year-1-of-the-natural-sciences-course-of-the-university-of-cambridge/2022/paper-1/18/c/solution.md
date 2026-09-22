<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand the right-hand side in the [orthonormal basis](../../../../../orthonormal-basis.md) from part (b). Its coefficients are

$$
\mathbf b\cdot\mathbf e_0=0,\qquad\mathbf b\cdot\mathbf e_4=2\sqrt2,\qquad\mathbf b\cdot\mathbf e_6=\sqrt3.
$$

Thus $\mathbf b=2\sqrt2\mathbf e_4+\sqrt3\mathbf e_6$. If $\mathbf x=c_0\mathbf e_0+c_4\mathbf e_4+c_6\mathbf e_6$, then [matrix multiplication](../../../../../matrix-multiplication.md) gives $A\mathbf x=4c_4\mathbf e_4+6c_6\mathbf e_6$. Matching coefficients fixes $c_4=\sqrt2/2$ and $c_6=\sqrt3/6$, while $c_0$ is arbitrary. Consequently all solutions are

$$
\boxed{\mathbf x=\begin{pmatrix}2/3\\-1/3\\1/6\end{pmatrix}+t\begin{pmatrix}1\\1\\-2\end{pmatrix},\qquad t\in\mathbb R.}
$$

Geometrically, the solution set is an [affine line in a vector space](../../../../../affine-line-in-a-vector-space.md) parallel to the [kernel](../../../../../kernel-of-a-linear-map-split.md) of $A$. The zero [eigenvalue](../../../../../eigenvalue.md) makes the component in that direction invisible to $A$; the other two components are uniquely determined. The displayed particular solution is perpendicular to the [kernel](../../../../../kernel-of-a-linear-map-split.md), so it is also the point of this [line](../../../../../straight-line.md) closest to the origin.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
