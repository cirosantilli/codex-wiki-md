<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Quantum teleportation](../../../../../quantum-teleportation.md) transfers an unknown [qubit](../../../../../qubit.md) state using a previously shared [Bell pair](../../../../../bell-pair.md), local operations and two classical bits. It requires no description of the unknown complex amplitudes and produces no extra copy.

Let the input be $|\chi\rangle_S=\alpha|0\rangle+\beta|1\rangle$, and let Alice and Bob share $|\Phi^+\rangle_{AB}$. Alice applies a [controlled-NOT gate](../../../../../controlled-not-gate.md) from $S$ to $A$, then a [Hadamard gate](../../../../../hadamard-gate.md) to $S$. Expanding the circuit gives the [Bell-basis teleportation identity](../../../../../bell-basis-teleportation-identity.md) in computational-output form:

$$
|\chi\rangle_S|\Phi^+\rangle_{AB}\longmapsto\frac12\sum_{a,b\in\{0,1\}}|a\rangle_S|b\rangle_A\,X^bZ^a|\chi\rangle_B.
$$

Her [projective measurement](../../../../../projective-measurement.md) yields each bit pair $(a,b)$ with probability $1/4$. She sends the two classical bits, and Bob applies **$Z^aX^b$** to recover $|\chi\rangle$. The order is the inverse of the displayed conditional operator; interchanging these Pauli corrections changes only an irrelevant global phase when both bits are one.

Before receiving the bits, Bob has

$$
\rho_B=\frac14\sum_{a,b}X^bZ^a|\chi\rangle\langle\chi|Z^aX^b=\frac I2.
$$

Thus teleportation respects the [no-communication theorem](../../../../../no-communication-theorem.md) and cannot transmit the usable unknown state faster than the classical message. Alice's input has been measured, and the shared entanglement resource has been consumed, in agreement with the [no-cloning theorem](../../../../../no-cloning-theorem.md). The protocol transfers the state, not the material particle initially carrying it.

A physical implementation must distribute and preserve an entangled pair, implement a Bell-basis measurement and transmit its result to a controllable output system. Imperfect entanglement, lost outcomes and noisy corrections reduce [quantum fidelity](../../../../../fidelity-of-quantum-states.md); a heralded probabilistic experiment must report its success probability separately from conditional fidelity. Ideal deterministic teleportation assumes every Bell outcome can be identified and corrected.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the quantum information course of the University of Cambridge](../../../../split.md)
6. [Quantum Information course of the University of Cambridge](../../../../../quantum-information-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
