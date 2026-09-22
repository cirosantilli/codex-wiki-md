<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

Let $H$ be a [Hermitian matrix](../../../../../hermitian-operator.md) and $He=\lambda e$ with $e\ne0$. The [inner product](../../../../../inner-product.md) $e^\dagger He$ is real because its conjugate equals $e^\dagger H^\dagger e=e^\dagger He$. But it also equals $\lambda e^\dagger e$, with $e^\dagger e>0$. Thus every [eigenvalue](../../../../../eigenvalue.md) is real. For two [eigenvectors](../../../../../eigenvector.md),

$$
e_i^\dagger He_j=\lambda_j e_i^\dagger e_j
=(He_i)^\dagger e_j=\lambda_i e_i^\dagger e_j.
$$

When $\lambda_i\ne\lambda_j$, this proves $e_i^\dagger e_j=0$, so the [eigenvectors](../../../../../eigenvector.md) are orthogonal.

For a real [antisymmetric matrix](../../../../../skew-symmetric-matrix.md), $(iA)^\dagger=-iA^T=iA$, so $iA$ is a [Hermitian matrix](../../../../../hermitian-operator.md). Its real [eigenvalues](../../../../../eigenvalue.md) imply that the [eigenvalues](../../../../../eigenvalue.md) of $A$ are purely imaginary. To ensure a nonzero one without assuming it, write

$$
A=\begin{pmatrix}0&-w_3&w_2\\w_3&0&-w_1\\-w_2&w_1&0\end{pmatrix},\qquad w\ne0.
$$

Expansion of the [characteristic polynomial](../../../../../characteristic-polynomial.md) gives $\det(tI-A)=t(t^2+|w|^2)$. Therefore the nonzero [eigenvalue](../../../../../eigenvalue.md) $-i\theta$ exists with $\theta=|w|>0$, and a nonzero complex [eigenvector](../../../../../eigenvector.md) $e_1=u+iv$ satisfies

$$
A(u+iv)=-i\theta(u+iv)=\theta v-i\theta u.
$$

Separating real and imaginary parts gives

$$
\boxed{Au=\theta v,\qquad Av=-\theta u.}
$$

Neither real vector can vanish, since either vanishing would force the other to vanish. Antisymmetry yields $0=u\cdot Au=\theta u\cdot v$ and

$$
-\theta|u|^2=u\cdot Av=-(Au)\cdot v=-\theta|v|^2.
$$

Thus $u,v$ are orthogonal and have equal length.

In odd dimension $\det A=\det A^T=\det(-A)=-\det A$, so $\det A=0$. Its real homogeneous system therefore has a nonzero real [eigenvector](../../../../../eigenvector.md) $e_3$ with $Ae_3=0$. It is perpendicular to $u,v$, because $e_3\cdot Au=-(Ae_3)\cdot u=0$ and similarly for $Av$. Normalize it and choose its sign so $(u/|u|,v/|v|,e_3)$ is positively oriented; this is an [orthonormal basis](../../../../../orthonormal-basis.md).

The [matrix exponential](../../../../../matrix-exponential.md) series converges absolutely, allowing even and odd terms to be grouped. Since $A^2u=-\theta^2u$ and $A^2v=-\theta^2v$, it acts as

$$
Ru=u\cos\theta+v\sin\theta,\qquad
Rv=v\cos\theta-u\sin\theta,\qquad Re_3=e_3.
$$

Consequently the [skew-symmetric exponential as an axial rotation](../../../../../skew-symmetric-exponential-as-an-axial-rotation.md) has, in the displayed [orthonormal basis](../../../../../orthonormal-basis.md), the matrix

$$
\boxed{\begin{pmatrix}\cos\theta&-\sin\theta&0\\\sin\theta&\cos\theta&0\\0&0&1\end{pmatrix}.}
$$

It is orthogonal with determinant one, fixes its axis and rotates the perpendicular plane. Hence **$R=e^A$ is a rotation matrix**, with angle $\theta$ about the chosen oriented axis.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
