<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the system's $z$ basis as $|0\rangle,|1\rangle$, and use a separate pair of meter [qubits](../../../../../../qubit.md) in the [Bell state](../../../../../../bell-state-split.md) $|\Phi^+\rangle$. Alice applies a [CNOT gate](../../../../../../controlled-not-gate.md) from system $A$ to her meter qubit; Bob simultaneously applies a [CNOT gate](../../../../../../controlled-not-gate.md) from $B$ to his meter qubit. Flipping neither or both meter qubits preserves $|\Phi^+\rangle$, while flipping exactly one gives $|\Psi^+\rangle$. Hence the [entanglement-assisted nondemolition parity measurement](../../../../../../entanglement-assisted-nondemolition-parity-measurement.md) interaction produces

$$
|\psi\rangle|\Phi^+\rangle\longmapsto
P_{\rm e}|\psi\rangle|\Phi^+\rangle+P_{\rm o}|\psi\rangle|\Psi^+\rangle,
$$

where $P_{\rm e}=|00\rangle\langle00|+|11\rangle\langle11|$ and $P_{\rm o}=|01\rangle\langle01|+|10\rangle\langle10|$. Each party now measures only their meter qubit in the $z$ basis. If their binary records are $u,v$, the system [Kraus operator](../../../../../../kraus-operator.md) is

$$
K_{uv}=\frac1{\sqrt2}P_{u\mathbin\oplus v},\qquad P_0=P_{\rm e},\quad P_1=P_{\rm o}.
$$

Unequal records verify zero total $z$ spin, since $S_z^{\rm tot}=\hbar(Z_A+Z_B)/2$ vanishes precisely on the odd sector. The probability of success is $\langle\psi|P_{\rm o}|\psi\rangle$, and the successful conditional state is $P_{\rm o}|\psi\rangle/\sqrt{\langle P_{\rm o}\rangle}$. **Every zero-total-$z$-spin state is left unchanged**, including any coherent superposition of $|01\rangle$ and $|10\rangle$. Similarly the even-sector coherence is preserved. This is a [quantum nondemolition measurement](../../../../../../quantum-nondemolition-measurement.md) of the parity, rather than separate measurements of both system spins.

All quantum operations and local meter measurements can finish within the spacelike time window. Nevertheless each local meter record is individually uniform: $K_{u0}^\dagger K_{u0}+K_{u1}^\dagger K_{u1}=I/2$. The verification result is obtained only by comparing the records using [local operations and classical communication](../../../../../../local-operations-and-classical-communication.md). Thus “instantaneous” refers to the local completion of the joint measurement instrument, not instant access to its nonlocal outcome; [quantum no-signalling](../../../../../../quantum-no-signalling.md) remains intact.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
