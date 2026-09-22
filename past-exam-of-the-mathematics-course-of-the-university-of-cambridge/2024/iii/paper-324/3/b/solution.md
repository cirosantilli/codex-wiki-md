<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The operators $X_i$ act on different [qubits](../../../../../../qubit.md) and therefore [commute](../../../../../../commuting-operators.md), so

$$
e^{-itJ_X}=\prod_{i=1}^ne^{-itX_i}.
$$

Since $X=HZH$,

$$
e^{-itX}=H e^{-itZ}H
=e^{-it}H\operatorname{diag}(1,e^{2it})H.
$$

The scalar $e^{-it}$ is a [global phase](../../../../../../global-phase.md). Thus each factor uses two [Hadamard gates](../../../../../../hadamard-gate.md) and one [phase gate](../../../../../../phase-gate.md), and applying the factors in parallel or sequentially gives an exact [quantum circuit](../../../../../../quantum-circuit-split.md) of $\boxed{3n}$ elementary gates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
