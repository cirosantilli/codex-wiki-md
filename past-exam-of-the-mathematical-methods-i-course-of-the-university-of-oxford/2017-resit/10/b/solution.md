<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [quadratic form](../../../../quadratic-form-split.md) has [symmetric matrix](../../../../symmetric-matrix.md)

$$
M=\begin{pmatrix}2&2\\2&-1\end{pmatrix},\qquad
\det(M-\lambda I)=\lambda^2-\lambda-6=(\lambda-3)(\lambda+2).
$$

Normalized [eigenvectors](../../../../eigenvector.md) for $3$ and $-2$ are $(2,1)/\sqrt5$ and $(-1,2)/\sqrt5$. They form the columns of the [rotation matrix](../../../../rotation-matrix.md)

$$
Q=\frac1{\sqrt5}\begin{pmatrix}2&-1\\1&2\end{pmatrix},\qquad
\binom xy=Q\binom{x'}{y'},\qquad
Q^TMQ=D=\boxed{\begin{pmatrix}3&0\\0&-2\end{pmatrix}}.
$$

Thus the new $x'$ axis is rotated counterclockwise by $\theta=\arctan(1/2)$, with

$$
\boxed{\sin\theta=\frac1{\sqrt5},\qquad f=3x'^2-2y'^2.}
$$

The opposite signs of the [eigenvalues](../../../../eigenvalue.md) classify each positive level as a [hyperbola](../../../../hyperbola.md). For the original level six its standard equation is $x'^2/2-y'^2/3=1$; for the final level one it is $3x'^2-2y'^2=1$. The printed change of level therefore changes the scale, but not the principal axes or [asymptotes](../../../../asymptote.md).

Setting the homogeneous quadratic part to zero gives $y'=\pm\sqrt{3/2}\,x'$. In the original coordinates put $y=mx$ in $2x^2+4xy-y^2=0$, obtaining

$$
\boxed{m=2\pm\sqrt6.}
$$

These are the slopes in the original $(x,y)$ axes; $\pm\sqrt{3/2}$ are the slopes in the rotated axes, so they must not be interchanged.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
