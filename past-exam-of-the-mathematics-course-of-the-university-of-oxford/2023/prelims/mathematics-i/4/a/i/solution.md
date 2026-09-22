<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

The real [spectral theorem](../../../../../../../spectral-theorem.md) states that a [symmetric matrix](../../../../../../../symmetric-matrix.md) has an [orthonormal basis](../../../../../../../orthonormal-basis.md) of real [eigenvectors](../../../../../../../eigenvector.md), and hence is a [diagonalisable matrix](../../../../../../../diagonalizable-matrix.md). Here is a proof in this setting.

For $n\ge1$, the [quadratic form](../../../../../../../quadratic-form-split.md) $q(x)=x^TAx$ attains a maximum on the [unit sphere](../../../../../../../unit-sphere.md), by [compactness](../../../../../../../compact-space.md) and the [extreme value theorem](../../../../../../../extreme-value-theorem.md). Choose a unit maximizer $u$ and put $\lambda=u^TAu$. For any $w\perp u$, the [Rayleigh quotient](../../../../../../../rayleigh-quotient.md) along $u+tw$ has a maximum at $t=0$, so

$$
0=\left.\frac{d}{dt}\frac{(u+tw)^TA(u+tw)}{\|u+tw\|^2}\right|_{t=0}
=2w^TAu.
$$

The last equality uses $A=A^T$ and $u^Tw=0$. Thus $Au$ is orthogonal to every $w\perp u$, so $Au=\lambda u$.

The [orthogonal complement](../../../../../../../orthogonal-complement.md) $u^\perp$ is an [invariant subspace](../../../../../../../invariant-subspace.md), because for $x\perp u$,

$$
u^TAx=(Au)^Tx=\lambda u^Tx=0.
$$

The [restriction](../../../../../../../restriction-mathematics.md) of $A$ to $u^\perp$ is again symmetric with respect to the induced [inner product](../../../../../../../inner-product-split.md). By [mathematical induction](../../../../../../../mathematical-induction.md) on [dimension](../../../../../../../dimension-vector-space.md), it has an [orthonormal basis](../../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../../eigenvector.md); adjoining $u$ gives one for $\mathbb R^n$. If $Q$ has those [basis vectors](../../../../../../../basis-vector.md) as columns, then $Q^TAQ$ is a real [diagonal matrix](../../../../../../../diagonal-matrix.md) and $Q^{-1}=Q^T$.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [4](../../../4.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
