<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Yes. Replace the target [qubit](../../../../qubit.md) by a register of $k$ [qubits](../../../../qubit.md) and implement the [controlled unitary gate](../../../../controlled-unitary-gate.md)

$$
C(U)=|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes U.
$$

The algebra in [c](../c.md) uses only normalization and [unitarity](../../../../unitary-operator.md), so for an arbitrary pure register [quantum state](../../../../quantum-state.md) $|\phi\rangle$ it still gives $\langle Z\rangle=\operatorname{Re}\langle\phi|U|\phi\rangle$. For a mixed register [quantum state](../../../../quantum-state.md) $\rho$, linearity gives $\operatorname{Re}\operatorname{Tr}(\rho U)$. With $\rho=I/2^k$,

$$
\boxed{\operatorname{Re}\operatorname{Tr}U=2^k(P_0-P_1).}
$$

Only the control [qubit](../../../../qubit.md) needs to be pure. A uniformly randomized [computational basis](../../../../computational-basis.md) preparation supplies the target [maximally mixed state](../../../../maximally-mixed-state.md). This is the principle of [trace estimation by a maximally mixed Hadamard test](../../../../trace-estimation-by-a-maximally-mixed-hadamard-test.md). The extension is algebraic; efficiently implementing controlled-$U$ still requires a known suitable gate construction. Moreover, estimating the unnormalized [trace](../../../../matrix-trace.md) to fixed additive precision requires increasingly precise estimation of the normalized signal as $k$ grows. There is no automatic efficient reconstruction of all entries of $U$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
