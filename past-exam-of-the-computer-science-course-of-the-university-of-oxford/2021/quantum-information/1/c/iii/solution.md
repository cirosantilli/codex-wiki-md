<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Charlie cannot send a [bit](../../../../../../bit.md) to Alice with the stated preparation, fixed interaction and final local measurements.** Write $V=\operatorname{CNOT}_{B\to A}$ and $W=\operatorname{CNOT}_{B\to C}$, so the complete gate is $U=WV$ with the rightmost gate acting first. Alice has finished interacting before the gate involving Charlie acts.

For arbitrary product input [density matrices](../../../../../../density-matrix-split.md), put $\tau_{AB}=V(\rho_A\otimes\rho_B)V^\dagger$. The final [reduced density matrix](../../../../../../reduced-density-matrix.md) of Alice is

$$
\rho_A'=\operatorname{Tr}_{BC}\!\left[W(\tau_{AB}\otimes\rho_C)W^\dagger\right]
=\operatorname{Tr}_{B}\tau_{AB}.
$$

The equality follows because a [unitary operator](../../../../../../unitary-operator.md) on the traced-out systems leaves the [partial trace](../../../../../../partial-trace.md) unchanged. The right-hand side is independent of Charlie's preparation. Therefore every outcome [probability](../../../../../../probability.md) of every local measurement by Alice is independent of Charlie's message. [Quantum no-signalling](../../../../../../quantum-no-signalling.md) applies after Alice's last interaction, even though [phase kickback](../../../../../../phase-kickback.md) can allow communication between the two [qubits](../../../../../../qubit.md) of an individual [CNOT gate](../../../../../../controlled-not-gate.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
