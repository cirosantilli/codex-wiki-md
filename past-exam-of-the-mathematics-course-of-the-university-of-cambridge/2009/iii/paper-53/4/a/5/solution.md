<h1 id="4/a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**A secure key can be produced, at one ideal secret bit per copy.** Denote Alice's additional flag qubit by $F$. Alice can measure $F$ in the [computational basis](../../../../../../../computational-basis.md) and, when its outcome is $1$, apply the [Pauli Z gate](../../../../../../../pauli-z-gate.md) to her half of the shared pair. The two flag outcomes each have [probability](../../../../../../../probability.md) $1/2$, and $Z_A|\Phi^-\rangle=|\Phi^+\rangle$; either branch therefore supplies the same pure [Bell pair](../../../../../../../bell-pair.md).

Equivalently, Alice applies the local controlled unitary

$$
U=I_{AB}\otimes|0\rangle\langle0|_F+(Z_A\otimes I_B)\otimes|1\rangle\langle1|_F.
$$

This [local flag correction of a Bell-state phase mixture](../../../../../../../local-flag-correction-of-a-bell-state-phase-mixture.md) changes the full [density matrix](../../../../../../../density-matrix.md) into

$$
\boxed{|\Phi^+\rangle\langle\Phi^+|_{AB}\otimes I_F/2.}
$$

The corrected pair is pure, so every purification factors between $AB$ and $FE$. Eve may know the flag without knowing the key bit obtained from $AB$. Alice need not disclose the flag, but even disclosing it does not compromise the corrected pure [Bell pair](../../../../../../../bell-pair.md). Tracing out the flag before correction would give the nonprivate mixture in the preceding case; retaining Alice's local side information is essential.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
