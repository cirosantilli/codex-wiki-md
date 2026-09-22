<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Use an [inner product](../../../../../inner-product.md) linear in its first argument. The [adjoint operator](../../../../../adjoint-operator.md) $\alpha^*$ is the unique [linear operator](../../../../../linear-operator.md) such that

$$
\langle\alpha v,w\rangle=\langle v,\alpha^*w\rangle\quad\text{for all }v,w\in V.
$$

In a finite-dimensional [inner product space](../../../../../inner-product-space.md), existence follows by choosing an [orthonormal basis](../../../../../orthonormal-basis.md): the [matrix](../../../../../matrix.md) of the adjoint is the conjugate transpose of the matrix of $\alpha$. Uniqueness follows from nondegeneracy of the [inner product](../../../../../inner-product.md).

If $\alpha(W)\subseteq W$, then for $w\in W$ and $v\in W^\perp$,

$$
\langle w,\alpha^*v\rangle=\langle\alpha w,v\rangle=0.
$$

Thus $\alpha^*v\in W^\perp$. Conversely, if $\alpha^*(W^\perp)\subseteq W^\perp$, the same equality gives $\langle\alpha w,v\rangle=0$ for every $v\in W^\perp$, so $\alpha w\in(W^\perp)^\perp=W$. This proves the [adjoint criterion for an invariant orthogonal complement](../../../../../adjoint-criterion-for-an-invariant-orthogonal-complement.md).

The equality $(W^\perp)^\perp=W$ uses the finite-dimensional setting appropriate here. In a general [Hilbert space](../../../../../hilbert-space-split.md) it holds for closed subspaces, and an adjoint is assured for bounded operators. Without closedness the converse only implies invariance of the closure. For example in $\ell^2$, take $W$ to be the finite-support sequences and $\alpha v=\langle v,e_1\rangle(2^{-j})_{j\geq1}$. Then $W^\perp=\{0\}$ is automatically adjoint-invariant, but $\alpha e_1\notin W$. Thus the finite-dimensional or closed-subspace hypothesis cannot be omitted from an infinite-dimensional reading.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
