<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

An always-on [Ising coupling](../../../../../../ising-coupling-of-two-qubits.md) produces evolution during every nominally local pulse, and generally does not commute with the applied $x,y$ [Quantum Hamiltonians](../../../../../../hamiltonian-quantum-mechanics.md). A naive product of single-[qubit](../../../../../../qubit.md) rotations therefore accumulates unwanted conditional phases and can entangle the qubits. Idling is also no longer an identity operation.

For a pulse of duration $\tau$, neglecting the coupling requires **$|J_{12}|\tau\ll1$** in units $\hbar=1$, or $|J_{12}|\tau/\hbar\ll1$ in ordinary units. For order-one rotation angles, this is the strong-local-drive regime $|B|\gg|J_{12}|$. Large drive amplitude alone does not justify neglect over a long total sequence: the accumulated interaction time or an appropriate error bound must also be small.

If it cannot be neglected, include it in the [quantum optimal control](../../../../../../quantum-optimal-control.md) model, or refocus it. A $\pi$ pulse $P=R_x^{(1)}(\pi)$ obeys $P(Z\otimes Z)P^\dagger=-Z\otimes Z$, giving the ideal [Ising spin echo](../../../../../../ising-spin-echo.md)

$$
e^{-iH_I\tau/2}P e^{-iH_I\tau/2}P^\dagger=I.
$$

This cancellation assumes the refocusing pulses are instantaneous relative to $1/|J_{12}|$, or that the coupling during finite pulses is compensated. It explains how fast local controls can suppress the fixed coupling without mistaking it for a controllable zero interaction.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
