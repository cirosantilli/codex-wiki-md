<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace every [CNOT gate](../../../../../../controlled-not-gate.md) by $H_jE_{ij}H_j$. The resulting [quantum circuit](../../../../../../quantum-circuit-split.md) contains only [Hadamard gates](../../../../../../hadamard-gate.md) and [Controlled-Z gates](../../../../../../controlled-z-gate.md). Realize each [Hadamard gate](../../../../../../hadamard-gate.md) by a fresh [one-bit teleportation](../../../../../../one-bit-teleportation.md) link measured at angle zero, so every internal measurement is in the fixed $X$ basis. Insert a graph edge between the current wire vertices for each [Controlled-Z gate](../../../../../../controlled-z-gate.md). This gives a suitable [graph state](../../../../../../graph-state.md) because the inputs are $|+\rangle$, and entangling gates can be moved to resource preparation: they commute with one another and with earlier measurements on vertices no longer used by the gate.

Track a [Pauli frame](../../../../../../pauli-frame.md) $\bigotimes_iX_i^{p_i}Z_i^{q_i}$. An angle-zero [one-bit teleportation](../../../../../../one-bit-teleportation.md) with raw result $s$ updates the frame on that wire by

$$
(p,q)\longmapsto(s\oplus q,p),
$$

because $HX^pZ^q$ equals $X^qZ^pH$ up to [global phase](../../../../../../global-phase.md). A [Controlled-Z gate](../../../../../../controlled-z-gate.md) updates $q_i\leftarrow q_i\oplus p_j$ and $q_j\leftarrow q_j\oplus p_i$, leaving the $p$ bits unchanged. These are classical binary updates; no measurement angle depends on them.

All the internal [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) consequently have predetermined bases. Their projectors act on distinct resource [vertices](../../../../../../vertex-graph-theory.md) and commute, so **all internal measurements can be performed simultaneously: the logical measurement depth is at most one**. If the output is to be read in the [computational basis](../../../../../../computational-basis.md), those fixed-basis measurements can occur in the same layer; a raw output $t_i$ is relabelled $t_i\oplus p_i$. If quantum outputs are retained, the same calculation gives the desired output in a known [Pauli frame](../../../../../../pauli-frame.md). This [nonadaptive Hadamard–CNOT measurement pattern](../../../../../../nonadaptive-hadamard-cnot-measurement-pattern.md) concerns measurement depth, not the depth of resource preparation or classical frame computation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
