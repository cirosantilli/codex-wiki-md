<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A square [complex matrix](../../../../complex-matrix.md) $U$ is a [unitary matrix](../../../../unitary-matrix.md) when $U^\dagger U=I$, so it preserves the [Euclidean norm](../../../../euclidean-norm.md). If $Uv=\mu v$ with $v\ne0$, then $\|v\|=\|Uv\|=|\mu|\|v\|$, giving **$|\mu|=1$**. For a [Hermitian matrix](../../../../hermitian-operator.md) $A=A^\dagger$ and $Ae_j=\lambda_je_j$,

$$
\lambda_j=\frac{e_j^\dagger Ae_j}{e_j^\dagger e_j}\in\mathbb R,
$$

because the numerator equals its complex conjugate. Hence no eigenvalue of $A+iI$ is zero, proving it is invertible.

For $V=(A-iI)(A+iI)^{-1}$, the [Hermitian conjugate](../../../../hermitian-conjugation.md) is $V^\dagger=(A-iI)^{-1}(A+iI)$. The factors and their inverses commute, since they are rational functions of $A$. Thus $V^\dagger V=I$. Its action on the same [eigenvectors](../../../../eigenvector.md) is

$$
\boxed{Ve_j=\frac{\lambda_j-i}{\lambda_j+i}e_j.}
$$

These eigenvalues have modulus one. This is the [Cayley transform of a Hermitian matrix](../../../../cayley-transform-of-a-hermitian-matrix.md) in the convention that avoids the unitary eigenvalue one.

For the inverse direction, $U^\dagger=U^{-1}$ gives

$$
(I-U^{-1})^{-1}=-(I-U)^{-1}U,\qquad I+U^{-1}=U^{-1}(I+U).
$$

Taking the conjugate transpose of $B=i(I+U)(I-U)^{-1}$ therefore yields

$$
B^\dagger=-i(I-U^{-1})^{-1}(I+U^{-1})=i(I-U)^{-1}(I+U)=B.
$$

The last equality uses commutativity of the two factors. This proves that the [inverse Cayley transform of a unitary matrix without eigenvalue one](../../../../inverse-cayley-transform-of-a-unitary-matrix-without-eigenvalue-one.md) is Hermitian. Solving for $U$ gives $U=(B-iI)(B+iI)^{-1}$. An orthonormal [eigenbasis](../../../../eigenbasis.md) of $B$ therefore diagonalizes $U$, with diagonal entries $(b_j-i)/(b_j+i)$.

The result extends even when a unitary matrix has eigenvalue one: choose $|\alpha|=1$ so that $\alpha U$ does not. There are only finitely many forbidden phases, since the matrix has finitely many [eigenvalues](../../../../eigenvalue.md). Diagonalizing $\alpha U$ also diagonalizes $U$ in the same basis. Thus **every unitary matrix is unitarily diagonalizable**.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
