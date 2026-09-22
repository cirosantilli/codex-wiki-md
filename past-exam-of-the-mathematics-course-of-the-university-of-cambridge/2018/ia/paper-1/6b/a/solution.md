<h1 id="6b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The characteristic polynomial of the displayed [rotation matrix](../../../../../../rotation-matrix.md) is $(1-\lambda)(\lambda^2-2\lambda\cos\theta+1)$, so its eigenvalues are $1,e^{i\theta},e^{-i\theta}$, all of [modulus](../../../../../../modulus.md) one. The real eigenvector $(0,0,1)^T$ spans the rotation axis, while the arguments $\pm\theta$ of the conjugate eigenvalues record the rotation angle on its perpendicular plane.

Applying first the $z$-rotation and then the $x$-rotation gives

$$
R_x(\pi/2)R_z(\pi/2)=
\begin{pmatrix}0&-1&0\\0&0&-1\\1&0&0\end{pmatrix}.
$$

Its $1$-eigenspace is spanned by $(1,-1,1)^T$, so $\mathbf n=(1,-1,1)^T/\sqrt3$. The [matrix trace](../../../../../../matrix-trace.md) identity $\operatorname{tr}R=1+2\cos\phi$ gives $0=1+2\cos\phi$. Thus **$\phi=2\pi/3$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6B](../../6b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
