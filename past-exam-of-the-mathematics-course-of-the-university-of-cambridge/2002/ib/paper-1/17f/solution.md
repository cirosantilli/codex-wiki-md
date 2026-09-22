<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

By orthogonal [diagonalization](../../../../../diagonalization-of-a-matrix.md) of the positive-definite [symmetric matrix](../../../../../symmetric-matrix.md) $A$, form its positive symmetric inverse square root $S=A^{-1/2}$. Then $S^TAS=I$, and $C=SBS$ is real symmetric. Let $Q$ have an orthonormal eigenbasis of $C$ as its columns, so $Q^TCQ=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$. Taking $P=SQ$ gives

$$
\boxed{P^TAP=I,\qquad P^TBP=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)}.
$$

Both factors of $P$ are invertible. This proves the [simultaneous congruence diagonalization with a positive form](../../../../../simultaneous-congruence-diagonalization-with-a-positive-form.md) by an explicit construction; it is congruence rather than simultaneous similarity.

To find the entries without constructing $P$, take determinants in

$$
P^T(B-\lambda A)P=\operatorname{diag}(\lambda_j-\lambda).
$$

Since $\det P\ne0$, the entries are precisely the roots, with multiplicity, of $\det(B-\lambda A)=0$. Equivalently they are the [eigenvalues](../../../../../eigenvalue.md) of $A^{-1}B$, although that matrix need not itself be symmetric.

For the given $A$, its leading principal minors are $2,3,4$, so it is positive definite. Expanding the [determinant](../../../../../determinant.md) gives

$$
\det(B-\lambda A)=\det\begin{pmatrix}4-2\lambda&-\lambda&0\\-\lambda&-2-2\lambda&-\lambda\\0&-\lambda&-2\lambda\end{pmatrix}=16\lambda+4\lambda^2-4\lambda^3.
$$

Thus the diagonal entries, in any order, are

$$
\boxed{0,\qquad\frac{1+\sqrt{17}}2,\qquad\frac{1-\sqrt{17}}2}.
$$

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
