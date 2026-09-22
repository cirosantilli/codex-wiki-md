<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Number the physical wires $1,\ldots,5$ from top to bottom and write a [computational basis](../../../../../../computational-basis.md) ket in that order. The first four are [ancilla qubits](../../../../../../ancilla-qubit.md) and the fifth carries the input. It is enough to follow the basis input $|b\rangle$, $b\in\{0,1\}$, because the encoding [quantum circuit](../../../../../../quantum-circuit-split.md) acts linearly.

The first fan-out consists of four [controlled-NOT gates](../../../../../../controlled-not-gate.md) from wire 5 to wires 1–4. It sends $|0000b\rangle$ to $|bbbbb\rangle$. The three [Hadamard gates](../../../../../../hadamard-gate.md) then give

$$
\frac1{\sqrt8}\sum_{a,c,d\in\{0,1\}}(-1)^{b(a+c+d)}|acd\,bb\rangle.
$$

The two [Pauli X gates](../../../../../../pauli-x-gate.md) on wires 2 and 3, followed by a [Controlled-Z gate](../../../../../../controlled-z-gate.md) and the same two X gates, restore the bits but contribute $(-1)^{(1-c)(1-d)}$: the sign is negative exactly when the original bits on both wires were zero. Finally, the right-hand [controlled-NOT gates](../../../../../../controlled-not-gate.md) are $3\to4$, $2\to5$, $1\to4$ and $1\to5$. They leave the first three bits unchanged and turn the last two into $b\oplus a\oplus d$ and $b\oplus a\oplus c$. Thus

$$
\boxed{|b_L\rangle=\frac1{\sqrt8}\sum_{a,c,d\in\{0,1\}}(-1)^{b(a+c+d)+(1-c)(1-d)}|a,c,d,b\oplus a\oplus d,b\oplus a\oplus c\rangle.}
$$

Explicitly, the logical basis [quantum states](../../../../../../quantum-state.md) produced by the printed gates are

$$
\begin{aligned}
|0_L\rangle=\frac1{\sqrt8}\bigl(&-|00000\rangle+|00110\rangle+|01001\rangle+|01111\rangle\\
&-|10011\rangle+|10101\rangle+|11010\rangle+|11100\rangle\bigr),\\
|1_L\rangle=\frac1{\sqrt8}\bigl(&-|00011\rangle-|00101\rangle-|01010\rangle+|01100\rangle\\
&+|10000\rangle+|10110\rangle+|11001\rangle-|11111\rangle\bigr).
\end{aligned}
$$

Each has eight orthogonal terms of equal magnitude, and their supports are disjoint, so they are normalized and mutually orthogonal. The arbitrary input is therefore encoded as

$$
\boxed{\alpha|0\rangle+\beta|1\rangle\longmapsto\alpha|0_L\rangle+\beta|1_L\rangle.}
$$

This is a realization of the [five-qubit error correcting code](../../../../../../five-qubit-error-correcting-code.md). The input amplitudes and their relative [quantum phase](../../../../../../quantum-phase.md) are preserved in the logical subspace; the encoding is an entangled-state [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md), not five independent copies of the unknown input. The explicit signs and bit ordering above are fixed by this circuit, rather than by a convention for a different encoder.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
