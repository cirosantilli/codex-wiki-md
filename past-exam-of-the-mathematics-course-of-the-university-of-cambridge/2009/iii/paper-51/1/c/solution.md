<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

All four promised functions have $a=1$. Use [quadratic Boolean phase cancellation](../../../../../../quadratic-boolean-phase-cancellation.md): apply a [Controlled-Z gate](../../../../../../controlled-z-gate.md) to remove the phase $(-1)^{xy}$, then apply the [Walsh-Hadamard transform](../../../../../../walsh-hadamard-transform.md). With the rightmost gate acting first, choose

$$
\boxed{U=(H\otimes H)C_Z.}
$$

Because $C_Z^2=I$ and the [Controlled-Z gate](../../../../../../controlled-z-gate.md) commutes with the [Pauli Z gates](../../../../../../pauli-z-gate.md),

$$
(U\otimes I)|\psi_{1bcd}\rangle=(-1)^d|bc\rangle\otimes|-\rangle.
$$

The [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) consequently produces

$$
\begin{array}{c|cccc}
\text{oracle}&f_{1000}&f_{1011}&f_{1101}&f_{1111}\\\hline
\text{outcome}&00&01&10&11
\end{array}
$$

Each answer occurs with [probability](../../../../../../probability.md) one for its promised [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
