<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**They need a pre-shared entanglement resource that permits deterministic production of a Bell pair.** In particular, one shared [Bell pair](../../../../../../bell-pair.md) and two classical bits suffice for exact [quantum teleportation](../../../../../../quantum-teleportation.md). This condition is stronger than merely having some entanglement.

Let Alice's input be $|\psi\rangle_C=\alpha|0\rangle+\beta|1\rangle$, and let her system $A$ and Bob's system $B$ share $|\Phi^+\rangle_{AB}=(|00\rangle+|11\rangle)/\sqrt2$. Use the [Bell states](../../../../../../bell-state-split.md) $|\Phi^\pm\rangle=(|00\rangle\pm|11\rangle)/\sqrt2$ and $|\Psi^\pm\rangle=(|01\rangle\pm|10\rangle)/\sqrt2$. Direct expansion gives

$$
|\psi\rangle_C|\Phi^+\rangle_{AB}
=\frac12\left[
|\Phi^+\rangle_{CA}|\psi\rangle_B+
|\Phi^-\rangle_{CA}Z|\psi\rangle_B+
|\Psi^+\rangle_{CA}X|\psi\rangle_B+
|\Psi^-\rangle_{CA}XZ|\psi\rangle_B
\right].
$$

Alice performs a [projective measurement](../../../../../../projective-measurement.md) in this Bell basis and sends its two-bit outcome. Each outcome has probability $1/4$. Bob applies respectively $I,Z,X,ZX$, recovering $|\psi\rangle$ exactly, without either party knowing $\alpha,\beta$. Before he receives the outcome, his averaged state is $I/2$, so the protocol does not communicate without the classical message. Alice's measurement consumes the input and the shared entanglement.

For necessity, exact transmission of every pure qubit means the induced [quantum channel](../../../../../../quantum-channel.md) is the identity: pure-state projectors span the operator space, and a physical channel is linear. Alice can therefore prepare a Bell pair locally and transmit one half by the proposed protocol, leaving a Bell pair shared with Bob. The protocol would itself be a deterministic [local operations and classical communication](../../../../../../local-operations-and-classical-communication.md) conversion of their resource into a Bell pair. This proves the [exact teleportation resource criterion](../../../../../../exact-teleportation-resource-criterion.md). With no shared entanglement, it is impossible: local operations and classical communication preserve [separable quantum states](../../../../../../separable-quantum-state.md), whereas the resulting Bell pair would be entangled.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
