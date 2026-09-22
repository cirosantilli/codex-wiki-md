<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Hadamard gate](../../../../../../hadamard-gate.md) identity $H=(X+Z)/\sqrt2$ on the first data wire. The $X_1$ branch is corrected as above and has syndrome $01$. The $Z_1$ branch changes the encoded state to $\alpha|000\rangle-\beta|111\rangle$, with syndrome $00$. No bit-flip recovery is triggered, and decoding leaves $Z|\psi\rangle$ on the top wire.

By linearity of the full [quantum circuit](../../../../../../quantum-circuit-split.md), its output for $H_1$ is therefore

$$
\frac1{\sqrt2}\left(|\psi\rangle\otimes|0001\rangle+Z|\psi\rangle\otimes|0000\rangle\right),
$$

where the four-bit strings are ordered as wires $2,3,4,5$. The two syndrome states are orthogonal. Taking their [partial trace](../../../../../../partial-trace.md) removes the cross terms, so the [reduced density matrix](../../../../../../reduced-density-matrix.md) is

$$
\rho=\frac12\left(|\psi\rangle\langle\psi|+Z|\psi\rangle\langle\psi|Z\right)
=\boxed{\begin{pmatrix}|\alpha|^2&0\\0&|\beta|^2\end{pmatrix}.}
$$

The top output undergoes a [completely dephasing channel](../../../../../../rank-one-dephasing.md) in the computational basis. The bit-flip component is corrected, but the undetected phase component destroys logical coherence after the syndrome is ignored.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
