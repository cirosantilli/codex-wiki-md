<h1 id="5f/solution">Solution</h1>

↑ **Parent:** [5F](../5f.md)

An [eigenvalue](../../../../../eigenvalue.md) of $C$ is a scalar $\lambda$ for which a nonzero vector $v$ satisfies $Cv=\lambda v$. Equivalently, $\det(\lambda I-C)=0$, because the homogeneous linear system has a nontrivial solution exactly when its coefficient [matrix](../../../../../matrix.md) is singular. This [characteristic polynomial](../../../../../characteristic-polynomial.md) is the monic quadratic

$$
\lambda^2-(\operatorname{tr}C)\lambda+\det C.
$$

A nonzero quadratic has at most two distinct roots, proving the [eigenvalue](../../../../../eigenvalue.md) bound. [Eigenvalues](../../../../../eigenvalue.md) and diagonalization are taken over $\mathbb C$, also for a [matrix](../../../../../matrix.md) with real entries.

For the [matrix commutator](../../../../../commutator.md), the cyclic [trace](../../../../../matrix-trace.md) identity follows directly from its entries:

$$
\operatorname{tr}(AB)=\sum_{i,j}A_{ij}B_{ji}
=\sum_{i,j}B_{ij}A_{ji}=\operatorname{tr}(BA).
$$

Hence **$\operatorname{tr}[A,B]=0$**. Factoring the [characteristic polynomial](../../../../../characteristic-polynomial.md) as $(\lambda-\lambda_1)(\lambda-\lambda_2)$ and comparing the coefficient of $\lambda$ gives **$\operatorname{tr}C=\lambda_1+\lambda_2$**, with the [eigenvalues](../../../../../eigenvalue.md) counted with algebraic multiplicity. If both [eigenvalues](../../../../../eigenvalue.md) are zero, [trace](../../../../../matrix-trace.md) and [determinant](../../../../../determinant.md) are zero. The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) then gives **$C^2=0$**; no diagonalizability assumption is needed.

Now put $M=[A,B]$. Since its [trace](../../../../../matrix-trace.md) is zero, its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2+\det M$ and the [scalar square of a traceless two-by-two matrix](../../../../../scalar-square-of-a-traceless-two-by-two-matrix.md) identity gives

$$
\boxed{[A,B]^2=\alpha I,\qquad \alpha=-\det[A,B]
=\frac12\operatorname{tr}([A,B]^2).}
$$

This proves the scalar-square assertion for both real and complex entries. If $\det M=0$, it gives $M^2=0$. If $\det M\ne0$, the two [eigenvalues](../../../../../eigenvalue.md) are the distinct nonzero numbers $\pm\sqrt{-\det M}$. Their eigenvectors are [linearly independent](../../../../../linear-independence.md): a nonzero vector cannot satisfy two different [eigenvalue](../../../../../eigenvalue.md) equations. They form a [basis](../../../../../basis.md), making $M$ a [diagonalizable matrix](../../../../../diagonalizable-matrix.md). Thus **either the commutator is diagonalizable over $\mathbb C$ or its square is zero**. These alternatives need not be disjoint, since the zero [matrix](../../../../../matrix.md) has both properties. Over $\mathbb R$ the diagonalization assertion would require real [eigenvalues](../../../../../eigenvalue.md); complex diagonalization is essential to the unrestricted statement.

## ↑ Ancestors (10)

1. [5F](../5f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
