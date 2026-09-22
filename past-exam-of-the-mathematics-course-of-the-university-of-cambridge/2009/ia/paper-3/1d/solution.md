<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

For a line through the origin making angle $\theta$ with the positive $x$-axis, its [reflection matrix](../../../../../reflection-matrix.md) is

$$
S_\theta=\begin{pmatrix}\cos2\theta&\sin2\theta\\\sin2\theta&-\cos2\theta\end{pmatrix}.
$$

Its [determinant](../../../../../determinant.md) is $-1$. An [orthogonal matrix](../../../../../orthogonal-matrix.md) has [determinant](../../../../../determinant.md) $\pm1$. If its [determinant](../../../../../determinant.md) is $-1$, write its first column as $(\cos\varphi,\sin\varphi)^T$; orthonormality and the [determinant](../../../../../determinant.md) then force the second column to be $(\sin\varphi,-\cos\varphi)^T$. The matrix is $S_{\varphi/2}$, hence is one [Euclidean reflection](../../../../../reflection-mathematics.md). If its [determinant](../../../../../determinant.md) is $+1$, the second column is $(-\sin\varphi,\cos\varphi)^T$, so it is a [rotation matrix](../../../../../rotation-matrix.md). Direct multiplication gives

$$
\boxed{R_\varphi=S_{\varphi/2}S_0.}
$$

The identity may be taken as an empty product or as two identical reflections. Thus at most two origin-line reflections suffice in every case.

For a nonzero vector $b=d n$ with $d=|b|$ and unit normal $n$, reflection in the affine line $n\cdot x=c$ is $s_c(x)=x+2(c-n\cdot x)n$. Consequently $s_{d/2}s_0(x)=x+d n=x+b$. A [translation](../../../../../translation-geometry.md) is therefore a product of two parallel-line reflections. Combining this with the given decomposition of a [Euclidean isometry](../../../../../euclidean-isometry.md) as translation followed by an orthogonal map proves that every plane isometry is a finite product of affine-line reflections. The affine lines need not pass through the origin. In fact three suffice: if an isometry $f$ sends zero to $b\ne0$, reflection in the perpendicular bisector of $0,b$ takes $b$ to zero. Composing that reflection with $f$ gives an isometry fixing zero, to which the two-reflection linear result applies. This is the planar [finite reflection decomposition of a Euclidean isometry](../../../../../finite-reflection-decomposition-of-a-euclidean-isometry.md).

For an example that genuinely needs three, take the [glide reflection](../../../../../glide-reflection.md)

$$
\boxed{g(x,y)=(x+1,-y).}
$$

It has no fixed point, so it is not one reflection. Its orthogonal part has [determinant](../../../../../determinant.md) $-1$, whereas the product of two reflections has [determinant](../../../../../determinant.md) $+1$, so it is not two reflections; it is not the identity either. Explicitly it is reflection in $y=0$ followed by reflection in $x=0$ and then in $x=1/2$. Thus its minimum reflection count is exactly three.

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
