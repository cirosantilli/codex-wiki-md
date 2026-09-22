<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An $n\times n$ [matrix](../../../../../matrix.md) is [diagonalizable](../../../../../diagonalizable-matrix.md) over a chosen field exactly when it has a basis of $n$ linearly independent [eigenvectors](../../../../../eigenvector.md). Equivalently, $P^{-1}AP$ is diagonal for some invertible $P$. Distinct [eigenvalues](../../../../../eigenvalue.md) suffice but are not necessary. For example,

$$
J=\begin{pmatrix}1&1\\0&1\end{pmatrix}
$$

is not diagonalizable: its only [eigenvalue](../../../../../eigenvalue.md) is $1$ and its [eigenspace](../../../../../eigenspace.md) is the one-dimensional span of $(1,0)^T$. It is a nontrivial [Jordan block](../../../../../jordan-block.md).

A [Hermitian matrix](../../../../../hermitian-operator.md) satisfies $A^\dagger=A$, where the dagger denotes [conjugate transpose](../../../../../conjugate-transpose.md). If $Av=\lambda v$ with $v\ne0$, then

$$
\lambda=\frac{v^\dagger Av}{v^\dagger v},\qquad
(v^\dagger Av)^*=v^\dagger A^\dagger v=v^\dagger Av.
$$

The denominator is positive real, so

$$
\boxed{\lambda\in\mathbb R.}
$$

For $Av=\lambda v$ and $Aw=\mu w$, Hermiticity also gives

$$
\mu v^\dagger w=v^\dagger Aw=(Av)^\dagger w=\lambda v^\dagger w.
$$

Thus

$$
\boxed{\lambda\ne\mu\quad\Longrightarrow\quad v^\dagger w=0.}
$$

This is the necessary qualification to the PDF's [orthogonality](../../../../../orthogonal-vectors.md) wording: arbitrary [eigenvectors](../../../../../eigenvector.md) belonging to a repeated [eigenvalue](../../../../../eigenvalue.md) need not be orthogonal. Within each repeated [eigenspace](../../../../../eigenspace.md), [Gram-Schmidt orthogonalization](../../../../../gram-schmidt-process.md) produces an orthonormal basis; together the [eigenspaces](../../../../../eigenspace.md) give an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) by the [finite-dimensional spectral theorem](../../../../../finite-dimensional-spectral-theorem.md). For example, $(1,0)^T$ and $(1,1)^T$ are nonorthogonal [eigenvectors](../../../../../eigenvector.md) of the identity [matrix](../../../../../matrix.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
