<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At $\theta=0$ the four [eigenstates](../../../../../../../eigenstate.md) are the computational product basis, with irrelevant signs on two vectors. Alice and Bob measure their own system qubits in $Z$. These local [projective measurements](../../../../../../../projective-measurement.md) preserve each product [eigenstate](../../../../../../../eigenstate.md); their pair of records identifies the global outcome after [local operations and classical communication](../../../../../../../local-operations-and-classical-communication.md).

At $\theta=\pi/4$ the four states are the [Bell states](../../../../../../../bell-state-split.md). They are simultaneous [eigenstates](../../../../../../../eigenstate.md) of the commuting [Pauli operators](../../../../../../../pauli-operator.md) $Z_AZ_B$ and $X_AX_B$: $\Phi^+,\Phi^-,\Psi^+,\Psi^-$ have respective pairs $(+,+),(+,-),(-,+),(-,-)$. Their nonlocal parity measurements can be performed without directly distinguishing the local system spins.

Use the first shared [Bell state](../../../../../../../bell-state-split.md) pair to perform the [entanglement-assisted nondemolition parity measurement](../../../../../../../entanglement-assisted-nondemolition-parity-measurement.md) of $Z_AZ_B$. Use the second shared pair for $X_AX_B$: both parties apply a local [Hadamard gate](../../../../../../../hadamard-gate.md) to their system qubit, execute the same local system-to-meter [CNOT gates](../../../../../../../controlled-not-gate.md) and $z$-meter measurements, then undo the [Hadamard gates](../../../../../../../hadamard-gate.md). This measures $X_AX_B$ because $HZH=X$. The two system parity projectors commute, since anticommutation at both sites cancels:

$$
[Z_AZ_B,X_AX_B]=0,\qquad
P_{z,x}=\frac14(I+zZ_AZ_B)(I+xX_AX_B),\quad z,x\in\{\pm1\}.
$$

Each $P_{z,x}$ is the corresponding rank-one [Bell state](../../../../../../../bell-state-split.md) projector. Every complete tuple of four local meter records has system [Kraus operator](../../../../../../../kraus-operator.md) $P_{z,x}/2$ for its two parities. Summing the four record tuples compatible with $(z,x)$ gives the ideal outcome map $\rho\mapsto P_{z,x}\rho P_{z,x}$. **The protocol is a Bell-state nondemolition measurement**: an input [Bell state](../../../../../../../bell-state-split.md) is preserved, while an arbitrary input is projected onto the reported [Bell state](../../../../../../../bell-state-split.md) with the [Born rule](../../../../../../../born-rule.md) probability.

The local circuits need no adaptive communication between the laboratories, so both parties can finish inside the specified time window. Global identification of $(z,x)$ still requires later [local operations and classical communication](../../../../../../../local-operations-and-classical-communication.md). This endpoint protocol respects [quantum no-signalling](../../../../../../../quantum-no-signalling.md), unlike the hypothetical intermediate-angle instrument in part (i).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
