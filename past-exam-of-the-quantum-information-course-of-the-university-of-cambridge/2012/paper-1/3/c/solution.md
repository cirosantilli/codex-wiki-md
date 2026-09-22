<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [quantum teleportation](../../../../../quantum-teleportation.md), Alice holds an unknown input $|\psi\rangle_1$ and one member of a shared $|\Phi^+\rangle_{23}$ pair; Bob holds [qubit](../../../../../qubit.md) 3. Alice applies a [CNOT gate](../../../../../controlled-not-gate.md) from 1 to 2 and a [Hadamard gate](../../../../../hadamard-gate.md) on 1, then measures both in the [computational basis](../../../../../computational-basis.md). Expansion gives the [Bell-basis teleportation identity](../../../../../bell-basis-teleportation-identity.md)

$$
(H_1\otimes I)\operatorname{CNOT}_{1\to2}
(|\psi\rangle_1|\Phi^+\rangle_{23})
=\frac12\sum_{m,n=0}^1|mn\rangle_{12}X^nZ^m|\psi\rangle_3.
$$

Every outcome pair $(m,n)$ has [probability](../../../../../probability.md) $1/4$, independently of the input. Alice sends these two classical bits, and Bob applies

$$
\boxed{Z^mX^n\,X^nZ^m|\psi\rangle=|\psi\rangle.}
$$

The order of the two corrections matters only by a global sign for the doubly nonzero outcome. The transformation also transfers entanglement with an untouched reference, because the identity is linear in the input amplitudes.

Before receiving the bits, Bob must average over all four Pauli-related states, obtaining $I/2$ for any input. Thus teleportation requires [classical communication](../../../../../classical-communication.md) and does not send information faster than light. The original input is consumed by Alice's measurement, so no second copy remains and the [no-cloning theorem](../../../../../no-cloning-theorem.md) is respected. Ideal [qubit](../../../../../qubit.md) teleportation consumes one shared Bell pair and two classical bits, as well as local gates and measurements. Imperfect entanglement, gate error, detection error or lost classical records reduce practical fidelity; teleportation transfers the [quantum state](../../../../../quantum-state.md), not the underlying material particle.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
