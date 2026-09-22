<h1 id="7b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $t\ne0$, factor the [matrix](../../../../../../matrix.md) as

$$
A^{-1}-tI=A^{-1}(I-tA)=A^{-1}\bigl[-t(A-t^{-1}I)\bigr].
$$

The [determinant](../../../../../../determinant.md) of a scalar multiple of an $n\times n$ [matrix](../../../../../../matrix.md) gains the scalar's $n$th power. Thus

$$
\boxed{\chi_{A^{-1}}(t)=(\det A)^{-1}(-1)^nt^n\chi_A(t^{-1}).}
$$

The right side extends to a [polynomial](../../../../../../polynomial-split.md) at $t=0$: multiplying $\chi_A(t^{-1})$ by $t^n$ removes all negative powers. Its value there is $(\det A)^{-1}$, since the leading coefficient of $\chi_A(s)=\det(A-sI)$ is $(-1)^n$. This equals $\chi_{A^{-1}}(0)$, so the identity holds at zero with that interpretation.

For the relation between [eigenvalues](../../../../../../eigenvalue.md) and the [characteristic polynomial](../../../../../../characteristic-polynomial.md),

$$
\lambda\text{ is an eigenvalue of }A
\iff \ker(A-\lambda I)\ne\{0\}
\iff A-\lambda I\text{ is singular}
\iff \chi_A(\lambda)=0.
$$

The first equivalence is the definition of an [eigenvector](../../../../../../eigenvector.md); the others use the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) and the criterion for an [invertible matrix](../../../../../../invertible-matrix.md) to have nonzero [determinant](../../../../../../determinant.md). Since $\chi_A$ has degree $n$, the [fundamental theorem of algebra](../../../../../../fundamental-theorem-of-algebra.md) gives $n$ roots over $\mathbb C$ counted with multiplicity. The multiplicity of a root is its [algebraic multiplicity](../../../../../../algebraic-multiplicity.md), and the [eigenspace](../../../../../../eigenspace.md) is exactly $\ker(A-\lambda I)$; its dimension is the [geometric multiplicity](../../../../../../geometric-multiplicity.md), which need not equal the [algebraic multiplicity](../../../../../../algebraic-multiplicity.md).

Finally, factor $p(s)=s^4-\mu$ over $\mathbb C$ as $p(s)=\prod_{j=1}^4(s-\lambda_j)$, including repeated roots when $\mu=0$. Substituting $A$ into this [polynomial](../../../../../../polynomial-split.md) is valid because the resulting factors commute. If $\mu$ is an [eigenvalue](../../../../../../eigenvalue.md) of $A^4$, then

$$
0=\det(A^4-\mu I)=\prod_{j=1}^4\det(A-\lambda_jI).
$$

At least one factor must be zero, so its $\lambda_j$ is an [eigenvalue](../../../../../../eigenvalue.md) of $A$ and satisfies $\lambda_j^4=\mu$. Thus the reverse direction of this instance of the [spectral mapping theorem](../../../../../../spectral-mapping-theorem.md) is

$$
\boxed{\mu\text{ an eigenvalue of }A^4
\ \Longrightarrow\ \exists\lambda\text{ an eigenvalue of }A\text{ with }\lambda^4=\mu.}
$$

This argument also covers $\mu=0$, when the conclusion is that $A$ is singular and has [eigenvalue](../../../../../../eigenvalue.md) zero.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
