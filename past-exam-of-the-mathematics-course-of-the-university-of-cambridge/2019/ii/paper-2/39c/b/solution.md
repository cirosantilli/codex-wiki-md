<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u_j=(u_{1,j},\ldots,u_{m,j})^T$ collect the unknowns in grid column $j$, and define $b_j=h^2(f_{1,j},\ldots,f_{m,j})^T$. The terms within one column form the block

$$
\boxed{B=\left[\frac23,-\frac{10}3,\frac23\right]},
$$

while coupling to either adjacent column contributes

$$
\boxed{C=\left[\frac16,\frac23,\frac16\right]}.
$$

The zero boundary values remove all blocks outside the displayed range, so the [nine-point finite-difference stencil](../../../../../../nine-point-finite-difference-stencil.md) becomes the [block tridiagonal matrix](../../../../../../block-tridiagonal-matrix.md) system

$$
\begin{pmatrix}
B&C&&\\
C&B&\ddots&\\
&\ddots&\ddots&C\\
&&C&B
\end{pmatrix}
\begin{pmatrix}u_1\\u_2\\\vdots\\u_m\end{pmatrix}
=
\begin{pmatrix}b_1\\b_2\\\vdots\\b_m\end{pmatrix}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
