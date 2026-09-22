<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Proceed by induction on $\dim V$. The result is immediate for dimension zero. In positive dimension, the [characteristic polynomial](../../../../../characteristic-polynomial.md) has a root over the [complex numbers](../../../../../complex-number.md), so there is a nonzero [eigenvector](../../../../../eigenvector.md) $v$ with [eigenvalue](../../../../../eigenvalue.md) $\lambda$. Normalize it to have norm one. [Self-adjointness](../../../../../self-adjoint-operator.md) gives

$$
\overline\lambda\langle v,v\rangle
=\langle Tv,v\rangle
=\langle v,Tv\rangle
=\lambda\langle v,v\rangle,
$$

so $\lambda$ is real.

The [orthogonal complement](../../../../../orthogonal-complement.md) $v^\perp$ is an [invariant subspace](../../../../../invariant-subspace.md): if $w\perp v$, then

$$
\langle v,Tw\rangle=\langle Tv,w\rangle
=\overline\lambda\langle v,w\rangle=0.
$$

The restriction of $T$ to $v^\perp$ is again [self-adjoint](../../../../../self-adjoint-operator.md), since the same [inner product](../../../../../inner-product-split.md) identity holds on that subspace. By induction it has an [orthonormal basis](../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../eigenvector.md). Adjoining $v$ gives

$$
\boxed{\text{an orthonormal basis of eigenvectors of $T$}.}
$$

The existence of the first [eigenvector](../../../../../eigenvector.md) is the essential use of the [complex numbers](../../../../../complex-number.md) in this proof of the finite-dimensional [spectral theorem](../../../../../spectral-theorem.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
