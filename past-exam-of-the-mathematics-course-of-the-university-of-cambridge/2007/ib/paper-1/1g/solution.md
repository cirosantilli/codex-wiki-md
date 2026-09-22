<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

In the given [basis](../../../../../basis.md), the [matrix](../../../../../matrix.md) is $A=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}$. Let $\omega=e^{2\pi i/3}$, a primitive cube [root of unity](../../../../../root-of-unity.md). For each $\xi\in\{1,\omega,\omega^2\}$,

$$
A\begin{pmatrix}1\\\xi\\\xi^2\end{pmatrix}
=\begin{pmatrix}\xi^2\\1\\\xi\end{pmatrix}
=\xi^2\begin{pmatrix}1\\\xi\\\xi^2\end{pmatrix}.
$$

Thus these are [eigenvectors](../../../../../eigenvector.md) with distinct [eigenvalues](../../../../../eigenvalue.md) $1,\omega^2,\omega$, respectively, and form an eigenbasis. Set

$$
P=\begin{pmatrix}1&1&1\\1&\omega&\omega^2\\1&\omega^2&\omega\end{pmatrix}.
$$

The columns are mutually orthogonal with squared norm three, so $P^{-1}=P^*/3$. **The [diagonalization](../../../../../diagonalization-of-a-matrix.md) and [characteristic polynomial](../../../../../characteristic-polynomial.md) are**

$$
\boxed{P^{-1}AP=\operatorname{diag}(1,\omega^2,\omega),\qquad
\chi_A(t)=\det(tI-A)=(t-1)(t-\omega)(t-\omega^2)=t^3-1.}
$$

Scaling $P$ by $1/\sqrt3$ gives a unitary diagonalizing [matrix](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
