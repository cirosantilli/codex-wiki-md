<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [characteristic polynomial](../../../../../../characteristic-polynomial.md) is

$$
\det(A-\lambda I)=(2-\lambda)(10-\lambda)-9
=\lambda^2-12\lambda+11=(\lambda-1)(\lambda-11).
$$

Thus the [eigenvalues](../../../../../../eigenvalue.md) are 1 and 11. Corresponding [eigenvectors](../../../../../../eigenvector.md) are $(3,-1)^T$ and $(1,3)^T$. Their dot product is zero and each has [Euclidean norm](../../../../../../euclidean-norm.md) $\sqrt{10}$. Normalizing gives

$$
\boxed{P=\frac1{\sqrt{10}}\begin{pmatrix}3&1\\-1&3\end{pmatrix},\qquad
D=\begin{pmatrix}1&0\\0&11\end{pmatrix}.}
$$

The columns are [orthonormal](../../../../../../orthonormal-set.md), so $P^TP=I$. The [eigenvector](../../../../../../eigenvector.md) equations give $AP=PD$ and hence $P^TAP=D$, proving the claimed [orthogonal diagonalization of a real symmetric matrix](../../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof resit](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
