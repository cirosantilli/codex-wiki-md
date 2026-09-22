<h1 id="8c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A complex square [matrix](../../../../../../matrix.md) $U$ is a [unitary matrix](../../../../../../unitary-matrix.md) when $U^\dagger U=I$, equivalently $U^{-1}=U^\dagger$. Here $\dagger$ denotes the [adjoint matrix](../../../../../../conjugate-transpose.md), the conjugate transpose. Such a matrix preserves the standard complex [inner product](../../../../../../inner-product.md) and its [Euclidean norm](../../../../../../euclidean-norm.md).

A real [symmetric matrix](../../../../../../symmetric-matrix.md) $A$ is a [Hermitian matrix](../../../../../../hermitian-operator.md), so $A^\dagger=A$. For arbitrary complex $\mathbf x$,

$$
\begin{aligned}
|(A+iI)\mathbf x|^2
&=\mathbf x^\dagger(A-iI)(A+iI)\mathbf x\\
&=\mathbf x^\dagger(A^2+I)\mathbf x\\
&=|A\mathbf x|^2+|\mathbf x|^2.
\end{aligned}
$$

The imaginary cross terms cancel because $A$ is Hermitian. Reversing the signs gives the same identity:

$$
\boxed{|(A-iI)\mathbf x|^2=|(A+iI)\mathbf x|^2
=|A\mathbf x|^2+|\mathbf x|^2.}
$$

In particular, $(A+iI)\mathbf x=0$ implies $|\mathbf x|^2=0$, so $A+iI$ has zero [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md). It is a square matrix, and the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) therefore makes it invertible. The same argument proves invertibility of $A-iI$.

The proposed matrix

$$
U=(A-iI)(A+iI)^{-1}
$$

is consequently well-defined. For any $\mathbf y$, put $\mathbf x=(A+iI)^{-1}\mathbf y$. The two norm identities show directly that

$$
|U\mathbf y|=|(A-iI)\mathbf x|
=|(A+iI)\mathbf x|=|\mathbf y|.
$$

To verify the [unitary matrix](../../../../../../unitary-matrix.md) identity explicitly, take adjoints:

$$
U^\dagger=(A-iI)^{-1}(A+iI).
$$

The two shifts commute, because both are polynomials in $A$. Hence

$$
\begin{aligned}
U^\dagger U
&=(A-iI)^{-1}(A+iI)(A-iI)(A+iI)^{-1}\\
&=(A-iI)^{-1}(A-iI)(A+iI)(A+iI)^{-1}=I.
\end{aligned}
$$

Thus

$$
\boxed{(A-iI)(A+iI)^{-1}\ \text{is unitary}.}
$$

**The imaginary shifts are invertible, and their equal norm changes cancel in the quotient.** This is the [Cayley transform of a Hermitian matrix](../../../../../../cayley-transform-of-a-hermitian-matrix.md) in the $(A-iI)(A+iI)^{-1}$ convention.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8C](../../8c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
