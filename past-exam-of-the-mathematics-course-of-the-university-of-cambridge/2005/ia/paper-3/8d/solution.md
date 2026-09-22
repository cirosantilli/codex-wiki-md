<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

First $E=\ker(A+I)$ is a [linear subspace](../../../../../vector-subspace.md). To prove it is nonzero, use [orthogonality](../../../../../orthogonal-vectors.md) and $\det A=-1$:

$$
\det(A+I)=\det A\,\det(I+A^{-1})
=-\det(I+A^T)=-\det(A+I).
$$

Hence $\det(A+I)=0$. If $u\in E$ then $Au=-u$ also implies $A^Tu=-u$. For $x\perp E$,

$$
\langle Ax,u\rangle=\langle x,A^Tu\rangle=-\langle x,u\rangle=0,
$$

so $E^\perp$ is invariant. If $E$ had dimension two, its one-dimensional [orthogonal complement](../../../../../orthogonal-complement.md) would be invariant and $A$ would act there as a scalar $\eta=\pm1$. The [determinant](../../../../../determinant.md) would be $(-1)^2\eta=-1$, so $\eta=-1$, forcing $A=-I$. Dimension three also forces $A=-I$. Both contradict the hypothesis. Consequently

$$
\boxed{\dim E=1.}
$$

Choose an [orthonormal basis](../../../../../orthonormal-basis.md) beginning with a [unit vector](../../../../../unit-vector.md) in $E$ and followed by a basis of $\Pi=E^\perp$. In this basis the [orthogonal matrix](../../../../../orthogonal-matrix.md) has block form

$$
A\sim\begin{pmatrix}-1&0\\0&R\end{pmatrix},
\qquad R^TR=I_2,\qquad \det R=1.
$$

The first column of $R$ is some $(\cos\theta,\sin\theta)^T$. Its perpendicular unit second column with positive orientation must be $(-\sin\theta,\cos\theta)^T$. Thus the restriction is the plane [rotation](../../../../../rotation-mathematics.md)

$$
R=\begin{pmatrix}\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta\end{pmatrix}.
$$

[Trace](../../../../../matrix-trace.md) invariance gives $\operatorname{tr}A=-1+2\cos\theta$, proving

$$
\boxed{\cos\theta=\tfrac12(\operatorname{tr}A+1).}
$$

A [Euclidean reflection](../../../../../reflection-mathematics.md) in $\Pi$ fixes that plane pointwise and reverses $E$, so it occurs exactly when $R=I_2$. This is equivalent to $\cos\theta=1$, hence **exactly to $\operatorname{tr}A=1$**. Finally,

$$
\det(A-I)=(-2)\det(R-I_2)
=-2\bigl((\cos\theta-1)^2+\sin^2\theta\bigr)
=\boxed{4(\cos\theta-1)}.
$$

This exhibits the [three-dimensional improper orthogonal transformation](../../../../../three-dimensional-improper-orthogonal-transformation.md) as a [rotation](../../../../../rotation-mathematics.md) about the axis $E$ composed with [Euclidean reflection](../../../../../reflection-mathematics.md) in $\Pi$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
