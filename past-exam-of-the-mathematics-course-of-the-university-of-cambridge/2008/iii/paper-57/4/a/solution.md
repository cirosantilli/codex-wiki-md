<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label the control [qubits](../../../../../../qubit.md) by binary weight: the bit $x_n$ contributes $2^n$ to $x=\sum_{n=0}^{N-1}2^nx_n$. For each $n$, use that [qubit](../../../../../../qubit.md) as the control of the supplied controlled-$V^{2^n}$, with the same target [eigenstate](../../../../../../eigenstate.md) $|v_j\rangle$. The [controlled unitary gate](../../../../../../controlled-unitary-gate.md) acts by

$$
\frac{|0\rangle+|1\rangle}{\sqrt2}|v_j\rangle\longmapsto\frac{|0\rangle+e^{i2^n\phi_j}|1\rangle}{\sqrt2}|v_j\rangle,
$$

since $V^{2^n}|v_j\rangle=e^{i2^n\phi_j}|v_j\rangle$. The target remains unchanged after every application. Multiplying these factors gives

$$
\left[\bigotimes_{n=0}^{N-1}\frac{|0\rangle+e^{i2^n\phi_j}|1\rangle}{\sqrt2}\right]|v_j\rangle=\boxed{\frac1{\sqrt{2^N}}\sum_{x=0}^{2^N-1}e^{i\phi_jx}|x\rangle}\,|v_j\rangle.
$$

The ordering of the tensor factors is chosen to match the binary place values. Discarding the unchanged target leaves the required phase register. This uses [quantum phase kickback](../../../../../../phase-kickback.md) in the phase accumulation step of [quantum phase estimation](../../../../../../quantum-phase-estimation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
