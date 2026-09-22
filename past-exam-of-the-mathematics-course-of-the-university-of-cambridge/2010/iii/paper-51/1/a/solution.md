<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Quantum teleportation](../../../../../../quantum-teleportation.md) transfers an arbitrary unknown [qubit](../../../../../../qubit.md) state to a separated receiver while using [local operations and classical communication](../../../../../../local-operations-and-classical-communication.md), rather than sending that input qubit. Alice and Bob first share one [maximally entangled state](../../../../../../maximally-entangled-state.md) of two qubits, such as a [Bell pair](../../../../../../bell-pair.md); a shared [spin singlet state](../../../../../../spin-singlet-state.md) is equivalent after a known [local unitary operation](../../../../../../local-unitary-operation.md).

Alice performs a joint [Bell-basis measurement](../../../../../../bell-basis-measurement.md) on the input qubit and her half of the pair. There are four possible outcomes. Bob's conditional qubit is the input state transformed by a known [Pauli operator](../../../../../../pauli-operator.md) determined by that outcome. Alice sends the outcome as two classical bits, and Bob applies the inverse [Pauli operator](../../../../../../pauli-operator.md). Thus **one shared Bell pair and two classical bits, together with local measurement and correction, transmit one unknown qubit exactly**. The entangled resource is consumed.

The procedure does not produce a classical description of the unknown amplitudes and does not leave a second copy at Alice, so it respects the [no-cloning theorem](../../../../../../no-cloning-theorem.md). Before receiving the classical outcome, Bob's [reduced density matrix](../../../../../../reduced-density-matrix.md) is $I/2$, independent of the input; this respects the [no-communication theorem](../../../../../../no-communication-theorem.md). The next part proves the full identity-channel action, including inputs entangled with another system.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
