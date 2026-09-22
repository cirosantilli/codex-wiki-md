<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Let $Q\in\mathrm{SO}(3,\mathbb R)$. Since $Q^TQ=I$ and $\det Q=1$,

$$
\det(Q-I)=\det Q\,\det(I-Q^T)=\det(I-Q)=-\det(Q-I),
$$

so $\det(Q-I)=0$. Choose a [unit vector](../../../../../unit-vector.md) $e$ with $Qe=e$. Its [orthogonal complement](../../../../../orthogonal-complement.md) is an [invariant subspace](../../../../../invariant-subspace.md): for $v\perp e$, $e\cdot Qv=(Q^Te)\cdot v=e\cdot v=0$. In an [orthonormal basis](../../../../../orthonormal-basis.md) $(e,e_1,e_2)$, $Q$ therefore has a scalar block $1$ and a two-dimensional [orthogonal matrix](../../../../../orthogonal-matrix.md) block of [determinant](../../../../../determinant.md) one. Such a block has columns $(\cos\theta,\sin\theta)^T$ and $(-\sin\theta,\cos\theta)^T$. Consequently $Q$ is a [rotation in three dimensions](../../../../../rotation-in-three-dimensions.md) about the axis $\mathbb Re$ through angle $\theta$, including the identity when $\theta=0$.

To construct the [Householder reflections](../../../../../householder-transformation.md), let $S_0$ reflect in the plane spanned by $e,e_1$ and let $S_\psi$ reflect in the plane spanned by $e,\cos\psi\,e_1+\sin\psi\,e_2$. They fix $e$, while on $e^\perp$ their [matrices](../../../../../matrix.md) are

$$
S_0=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad S_\psi=\begin{pmatrix}\cos2\psi&\sin2\psi\\\sin2\psi&-\cos2\psi\end{pmatrix}.
$$

Their product is the planar [rotation matrix](../../../../../rotation-matrix.md) through $2\psi$. Taking $\psi=\theta/2$ proves $\boxed{Q=S_{\theta/2}S_0}$. This gives the [composition of two plane reflections](../../../../../composition-of-two-plane-reflections.md) explicitly; each is a [Householder reflection](../../../../../householder-transformation.md) $I-2nn^T$ for the corresponding unit plane normal $n$.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
