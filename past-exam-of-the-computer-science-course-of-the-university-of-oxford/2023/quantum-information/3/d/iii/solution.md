<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Combine the hypothetical protocol with [superdense coding](../../../../../../superdense-coding.md). Before a message is chosen, Alice and Bob share a further [Bell pair](../../../../../../bell-pair.md) $|\phi_+\rangle_{QR}$, with $Q$ at Alice and $R$ at Bob, in addition to any resources needed for the hypothetical [quantum teleportation](../../../../../../quantum-teleportation.md) protocol. To encode two classical [bits](../../../../../../bit.md) $u,v$, Alice applies the [Pauli gates](../../../../../../pauli-gate.md) $Z_Q^uX_Q^v$, preparing

$$
|\beta_{uv}\rangle_{QR}=(Z_Q^uX_Q^v\otimes I_R)|\phi_+\rangle_{QR}.
$$

The four choices are the four mutually [orthogonal](../../../../../../orthogonal-vectors.md) [Bell states](../../../../../../bell-state-split.md). Alice now uses the hypothetical protocol to teleport $Q$ to Bob using only one classical [bit](../../../../../../bit.md). Its assumed preservation of the joint [quantum state](../../../../../../quantum-state.md) gives Bob both $B$ and $R$ in

$$
|\beta_{uv}\rangle_{BR}=(Z_B^uX_B^v\otimes I_R)|\phi_+\rangle_{BR}.
$$

Bob performs a [Bell-basis measurement](../../../../../../bell-basis-measurement.md). Explicitly, a [controlled-NOT gate](../../../../../../controlled-not-gate.md) $B\to R$, followed by a [Hadamard gate](../../../../../../hadamard-gate.md) on $B$, gives

$$
\boxed{(H_B\otimes I_R)\operatorname{CNOT}_{B\to R}|\beta_{uv}\rangle_{BR}=|u\rangle_B|v\rangle_R.}
$$

A [computational-basis measurement](../../../../../../quantum-measurement-in-the-computational-basis.md) therefore recovers **both message bits with certainty after only one transmitted classical bit**. The initial [Bell pairs](../../../../../../bell-pair.md) are shared before the message is chosen and carry no message themselves. This proves the [classical communication lower bound for exact qubit teleportation](../../../../../../classical-communication-lower-bound-for-exact-qubit-teleportation.md): a perfect protocol preserving an external reference needs at least two transmitted classical [bits](../../../../../../bit.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
