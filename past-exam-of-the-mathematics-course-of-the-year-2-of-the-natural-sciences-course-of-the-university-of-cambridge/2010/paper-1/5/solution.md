<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [eigenvalue](../../../../eigenvalue.md) $\lambda$ and associated [eigenvector](../../../../eigenvector.md) $e\ne0$ satisfy $Ae=\lambda e$. The [characteristic polynomial](../../../../characteristic-polynomial.md) $\det(A-\lambda I)$ has degree equal to the positive [matrix](../../../../matrix.md) size. The [fundamental theorem of algebra](../../../../fundamental-theorem-of-algebra.md) gives a complex root, at which $A-\lambda I$ is singular and therefore has a nontrivial kernel. Hence every nonempty square complex [matrix](../../../../matrix.md) has an [eigenvector](../../../../eigenvector.md).

A nondiagonalizable example is the [Jordan block](../../../../jordan-block.md) $\begin{pmatrix}0&1\\0&0\end{pmatrix}$: its only [eigenvalue](../../../../eigenvalue.md) is zero, and its eigenspace is one-dimensional. A [Hermitian matrix](../../../../hermitian-operator.md) satisfies $A^\dagger=A$ and has an [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) by the [spectral theorem](../../../../spectral-theorem.md). One proof finds an [eigenvector](../../../../eigenvector.md), notes that its [orthogonal complement](../../../../orthogonal-complement.md) is invariant, and repeats. Its [eigenvalues](../../../../eigenvalue.md) are real because

$$
\lambda\,e^\dagger e=e^\dagger Ae=\overline{e^\dagger Ae}=\overline\lambda\,e^\dagger e,
$$

where $e^\dagger e>0$.

With all [eigenvalues](../../../../eigenvalue.md) negative, $A$ is invertible. Its same complete eigenbasis gives

$$
\boxed{A^{-1}e_i=\lambda_i^{-1}e_i,\qquad A^me_i=\lambda_i^me_i\quad(m=1,2,\ldots).}
$$

Some powered [eigenvalues](../../../../eigenvalue.md) can coincide, but the original [eigenvectors](../../../../eigenvector.md) remain a complete basis. Writing $A=U\operatorname{diag}(\lambda_i)U^\dagger$, the convergent [matrix exponential](../../../../matrix-exponential.md) series gives

$$
\int_0^\infty e^{tA}dt=U\operatorname{diag}\left(\int_0^\infty e^{t\lambda_i}dt\right)U^\dagger=U\operatorname{diag}(-\lambda_i^{-1})U^\dagger.
$$

Thus the [matrix inverse from a decaying matrix exponential](../../../../matrix-inverse-from-a-decaying-matrix-exponential.md) is

$$
\boxed{\int_0^\infty e^{tA}dt=-A^{-1},\qquad A^{-1}=-\int_0^\infty e^{tA}dt.}
$$

**The identity printed in the original PDF is missing a minus sign.** Already for the one-by-one [matrix](../../../../matrix.md) $A=(-1)$ its integral is $1$, whereas its inverse is $-1$. Equivalently, integrating $d(e^{tA})/dt=Ae^{tA}$ gives $A\int_0^\infty e^{tA}dt=-I$, confirming the correction without diagonalization.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
