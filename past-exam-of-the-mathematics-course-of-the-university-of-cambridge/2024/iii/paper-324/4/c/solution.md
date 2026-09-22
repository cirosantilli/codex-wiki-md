<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Implement the assumed efficient classical algorithm for $x\mapsto\theta_x$ as a [reversible circuit](../../../../../../reversible-circuit.md). On input $|x\rangle|0^s\rangle$, it computes an $O(m)$-bit [binary expansion](../../../../../../binary-expansion.md) of the angle in a work register using $\operatorname{poly}(m)$ [Toffoli gates](../../../../../../toffoli-gate.md) and elementary reversible gates. Write the computed angle as a sum of binary-weighted angles. For each angle bit, apply the corresponding controlled single-qubit $R_y$ rotation to the target. These rotations have the same axis, so their angles add and produce

$$
|x\rangle|\widetilde\theta_x\rangle
(\cos\theta_x|0\rangle+\sin\theta_x|1\rangle).
$$

Finally apply [uncomputation](../../../../../../uncomputation.md) to erase the work register. Each [Toffoli gate](../../../../../../toffoli-gate.md) and controlled rotation has a constant-size decomposition into one- and two-qubit gates when arbitrary one-qubit rotations are available. Ignoring the stipulated precision costs, the resulting circuit has size $\operatorname{poly}(m)$ and returns every [quantum ancilla](../../../../../../quantum-ancilla.md) to zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
