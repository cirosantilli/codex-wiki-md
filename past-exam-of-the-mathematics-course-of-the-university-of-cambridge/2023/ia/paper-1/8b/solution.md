<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

A real [matrix](../../../../../matrix.md) is orthogonal when $Q^TQ=I$. If $Qv=\lambda v$, norm preservation gives $|\lambda|=1$. If $Qv=\lambda v$ and $Qw=\mu w$, preservation of the Hermitian [inner product](../../../../../inner-product.md) gives $(1-\overline\lambda\mu)v^\dagger w=0$; distinct unit-modulus [eigenvalues](../../../../../eigenvalue.md) therefore have orthogonal [eigenvectors](../../../../../eigenvector.md).

The nonreal [eigenvalues](../../../../../eigenvalue.md) of a real $3\times3$ [matrix](../../../../../matrix.md) occur in conjugate pairs. Since their product is one and $\det Q=-1$, the remaining real [eigenvalue](../../../../../eigenvalue.md) is $-1$. If $x\cdot n=0$, then $(Qx)\cdot(Qn)=x\cdot n=0$, and $Qn=-n$, so $Qx\cdot n=0$: the plane $\Pi$ is invariant.

The restriction to $\Pi$ is a planar orthogonal map whose [determinant](../../../../../determinant.md) is $(-1)/(-1)=1$, hence a rotation through some $\theta$. In an orthonormal [basis](../../../../../basis.md) adapted to $n$,

$$
Q\sim\operatorname{diag}(-1,R_\theta).
$$

Therefore $\operatorname{tr}Q=-1+2\cos\theta$ and

$$
\boxed{\det(Q-I)=(-2)\det(R_\theta-I)=4(\cos\theta-1).}
$$

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
