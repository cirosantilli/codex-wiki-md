<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Reverse communication is also possible.** Prepare Alice in $|+\rangle_A$. Bob encodes $m=0$ as $|+\rangle_B$ and $m=1$ as $|-\rangle_B$. Since $X|\pm\rangle=\pm|\pm\rangle$, [phase kickback](../../../../../../phase-kickback.md) gives

$$
\operatorname{CNOT}_{A\to B}\bigl(|+\rangle_A|(-)^m\rangle_B\bigr)
=\frac{|0\rangle_A+(-1)^m|1\rangle_A}{\sqrt2}\otimes|(-)^m\rangle_B,
$$

where $|(-)^0\rangle=|+\rangle$ and $|(-)^1\rangle=|-\rangle$. Alice measures in the [Hadamard basis](../../../../../../hadamard-basis.md): $+$ means zero and $-$ means one, deterministically.

The target's [Pauli X gate](../../../../../../pauli-x-gate.md) [eigenvalue](../../../../../../eigenvalue.md) becomes a [relative phase](../../../../../../relative-quantum-phase.md) on the control. This is the operational content of [CNOT control reversal in the Hadamard basis](../../../../../../cnot-control-reversal-in-the-hadamard-basis.md); the [computational basis](../../../../../../computational-basis.md) control arrow alone does not determine every possible direction of communication.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
