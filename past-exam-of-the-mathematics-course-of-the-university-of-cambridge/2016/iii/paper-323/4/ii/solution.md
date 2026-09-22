<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The coefficient [matrix](../../../../../../matrix.md) in the [computational basis](../../../../../../computational-basis.md) is

$$
M=\frac1{\sqrt{15}}\begin{pmatrix}2\sqrt2&-1\\\sqrt2&2\end{pmatrix}.
$$

For a bipartite [pure state](../../../../../../pure-state.md), the [partial traces](../../../../../../partial-trace.md) give $\psi_A=MM^\dagger$ and $\psi_B=M^T\overline M$. Therefore **the requested reduced density matrices are**

$$
\boxed{\psi_A=\frac1{15}\begin{pmatrix}9&2\\2&6\end{pmatrix},\qquad
\psi_B=\frac1{15}\begin{pmatrix}10&0\\0&5\end{pmatrix}.}
$$

The columns of $M$ are orthogonal. Their norms are $\sqrt{2/3}$ and $\sqrt{1/3}$, so normalizing them gives the [orthonormal set](../../../../../../orthonormal-set.md)

$$
|u_0\rangle=\frac{2|0\rangle+|1\rangle}{\sqrt5},\qquad
|u_1\rangle=\frac{-|0\rangle+2|1\rangle}{\sqrt5}.
$$

With $|v_0\rangle=|0\rangle$ and $|v_1\rangle=|1\rangle$, a [Schmidt decomposition](../../../../../../schmidt-decomposition.md) is

$$
\boxed{|\psi\rangle=\sqrt{\frac23}|u_0\rangle|0\rangle+
\sqrt{\frac13}|u_1\rangle|1\rangle.}
$$

Expanding this expression reproduces the minus sign in the $|01\rangle$ coefficient. The two [reduced density matrices](../../../../../../reduced-density-matrix.md) both have [eigenvalues](../../../../../../eigenvalue.md) $2/3$ and $1/3$, consistent with these [Schmidt coefficients](../../../../../../schmidt-coefficient.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
