<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\lambda=e^{2\pi i\phi}$. In terms of the [Pauli X gate](../../../../../../pauli-x-gate.md), the given [unitary operator](../../../../../../unitary-operator.md) is $U_\phi=aI+bX$, with $a=(1+\lambda)/2$ and $b=(1-\lambda)/2$. Since $X|+\rangle=|+\rangle$ and $X|-\rangle=-|-\rangle$,

$$
\boxed{U_\phi|+\rangle=|+\rangle,\qquad U_\phi|-\rangle=e^{2\pi i\phi}|-\rangle.}
$$

Thus the normalized [eigenvectors](../../../../../../eigenvector.md) are $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$, with [eigenvalues](../../../../../../eigenvalue.md) $1$ and $e^{2\pi i\phi}$ respectively. At $\phi=0$ they coincide as eigenvalues, and the whole two-dimensional [Hilbert space](../../../../../../hilbert-space-split.md) is the eigenspace; the same chosen eigenbasis remains valid.

Prepare $|-\rangle$ independently of $\phi$ and use the [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md) circuit of the preceding parts on the controlled-$U_\phi$ black box. It returns $\phi$ exactly using

$$
\boxed{2^m-1=O(2^m)\text{ controlled black-box calls}.}
$$

The chosen eigenstate contains all the unknown phase information, unlike $|+\rangle$, whose eigenvalue is independent of $\phi$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
