<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In [superdense coding](../../../../superdense-coding.md), Alice applies a local [Pauli operator](../../../../pauli-operator.md) to her half of the shared [Bell state](../../../../bell-state-split.md). Choose a phase bit $u$ and a parity bit $v$, and encode them using $X^vZ^u$ on Alice's qubit. With the standard definitions of the [Bell states](../../../../bell-state-split.md),

$$
\begin{array}{c|c|c}
uv&\text{Alice's operator}&\text{Bell state, up to global phase}\\\hline
00&I&\Phi^+=(|00\rangle+|11\rangle)/\sqrt2\\
01&X&\Psi^+=(|01\rangle+|10\rangle)/\sqrt2\\
10&Z&\Phi^-=(|00\rangle-|11\rangle)/\sqrt2\\
11&XZ&\Psi^-=(|01\rangle-|10\rangle)/\sqrt2
\end{array}.
$$

Alice sends her [qubit](../../../../qubit.md) to Bob. He now holds both halves and performs a [Bell-basis measurement](../../../../bell-basis-measurement.md), recovering $uv$ without error. Equivalently, a [CNOT gate](../../../../controlled-not-gate.md) with Alice's qubit as control, followed by a [Hadamard gate](../../../../hadamard-gate.md) on that qubit, maps these states to their computational labels up to [global phases](../../../../global-phase.md). Four distinguishable alternatives give **two classical bits per transmitted qubit**, with one shared entangled pair consumed per use.

The initial entanglement distribution is independent of the later message and can be completed beforehand. Bob's local [reduced density matrix](../../../../reduced-density-matrix.md) before Alice's transmission is $I/2$ for every encoding, so [quantum no-signalling](../../../../quantum-no-signalling.md) prevents it from carrying her choice. This does not make the entangled pair free: if a qubit transmission is used to distribute it, counting that transmission as well gives two qubit transmissions for the two-bit message. The quoted dense-coding rate counts the subsequent message-bearing transmission with entanglement already shared.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [7](../../7-split.md)
3. [2006](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
