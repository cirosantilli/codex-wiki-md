<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Initialize the register in

$$
\boxed{|\phi_y\rangle=H^{\otimes N}|y\rangle=T_y|\phi\rangle.}
$$

This can be prepared by [Pauli X gates](../../../../../../pauli-x-gate.md) on the one-bits of $y$, starting from $|0^N\rangle$, followed by [Hadamard gates](../../../../../../hadamard-gate.md) on all [qubits](../../../../../../qubit.md). Alternatively, prepare the original uniform state and apply [Pauli Z gates](../../../../../../pauli-z-gate.md) at those same bit positions. The conjugation calculation gives

$$
G_y^n|\phi_y\rangle=T_yG^n|\phi\rangle.
$$

The final diagonal sign operator changes no [computational basis](../../../../../../computational-basis.md) outcome [probabilities](../../../../../../probability.md). Thus the success [probability](../../../../../../probability.md) and the iteration count in part (b) are unchanged. No final correction is needed when the objective is to measure a marked string.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
