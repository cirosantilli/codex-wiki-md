<h1 id="8b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First note that if $A$ is normal, then

$$
\|(A-\lambda I)v\|
=\|(A^\dagger-\overline\lambda I)v\|
$$

for every $v$. Hence an [eigenvector](../../../../../../eigenvector.md) $v$ with $Av=\lambda v$ also satisfies

$$
A^\dagger v=\overline\lambda v.
$$

Normalize $v$ and extend it to an orthonormal [basis](../../../../../../basis.md). Let $U$ have these [basis](../../../../../../basis.md) [vectors](../../../../../../vector.md) as columns. The first column of $U^\dagger AU$ is $(\lambda,0,\ldots,0)^T$. For every $w\perp v$,

$$
\langle v,Aw\rangle
=\langle A^\dagger v,w\rangle
=\langle\overline\lambda v,w\rangle=0,
$$

so the first row also has no off-diagonal entries. Therefore

$$
U^\dagger AU=
\begin{pmatrix}
\lambda&0\\
0&B
\end{pmatrix}.
$$

Comparing the two block products in the normality identity shows that $BB^\dagger=B^\dagger B$, so $B$ is normal.

The result is trivial in dimension one. Applying the induction hypothesis to $B$ and adjoining the [eigenvector](../../../../../../eigenvector.md) $v$ gives an orthonormal eigenbasis for $A$. This proves the [unitary diagonalization of a normal matrix](../../../../../../unitary-diagonalization-of-a-normal-matrix.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8B](../../8b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
