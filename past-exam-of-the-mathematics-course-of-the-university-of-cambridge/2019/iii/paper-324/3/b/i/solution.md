<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a clean [quantum ancilla](../../../../../../../quantum-ancilla.md) and apply the [quantum circuit](../../../../../../../quantum-circuit-split.md) $C$, then the [Pauli Z gate](../../../../../../../pauli-z-gate.md) on the ancilla, then the [inverse quantum circuit](../../../../../../../inverse-quantum-circuit.md) $C^\dagger$:

$$
|x,0\rangle\xrightarrow{C}|x,f(x)\rangle
\xrightarrow{I\otimes Z}(-1)^{f(x)}|x,f(x)\rangle
\xrightarrow{C^\dagger}(-1)^{f(x)}|x,0\rangle.
$$

This [compute-phase-uncompute construction](../../../../../../../compute-phase-uncompute-construction.md) implements $A\otimes I$ on every input with the ancilla initially $|0\rangle$, and by [linearity](../../../../../../../linearity.md) on any superposition of those inputs. The action on ancilla-$|1\rangle$ inputs need not coincide with $A\otimes I$; the question only requires the clean-ancilla subspace.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
