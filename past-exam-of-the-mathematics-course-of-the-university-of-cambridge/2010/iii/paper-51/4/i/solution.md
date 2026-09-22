<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Diagonalize the [density operator](../../../../../../density-matrix.md) in the [Hadamard gate](../../../../../../hadamard-gate.md) basis $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. Its eigenvalues are $2/3,1/3$, so

$$
\rho_A=\frac23|+\rangle\langle+|+\frac13|-\rangle\langle-|.
$$

Choose orthonormal records on a second qubit to construct the first [purification of a density operator](../../../../../../purification-of-a-density-operator.md):

$$
\boxed{|\Omega_1\rangle=\sqrt{\frac23}|+\rangle_A|0\rangle_B+\sqrt{\frac13}|-\rangle_A|1\rangle_B.}
$$

It is normalized. In its outer product the cross terms have partial trace zero because $\langle0|1\rangle_B=0$, while the diagonal terms give precisely $\rho_A$.

A different purification follows from [unitary freedom of purification](../../../../../../unitary-freedom-of-purification.md). Apply the [Hadamard gate](../../../../../../hadamard-gate.md) to $B$:

$$
\boxed{|\Omega_2\rangle=(I\otimes H)|\Omega_1\rangle
=\sqrt{\frac23}|+\rangle_A|+\rangle_B+\sqrt{\frac13}|-\rangle_A|-\rangle_B.}
$$

The same partial-trace calculation uses $\langle+|-\rangle_B=0$ and gives $\rho_A$. The two global states are distinct, not related by a global phase, although their reduced density operators agree. Explicitly the second is

$$
|\Omega_2\rangle=a(|00\rangle+|11\rangle)+b(|01\rangle+|10\rangle),\qquad
a=\frac{\sqrt2+1}{2\sqrt3},\quad b=\frac{\sqrt2-1}{2\sqrt3}.
$$

Its reduction has diagonal entries $a^2+b^2=1/2$ and off-diagonal entries $2ab=1/6$, checking all the required matrix entries.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
