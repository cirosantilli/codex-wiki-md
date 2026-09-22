<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $|\psi\rangle=a|0\rangle+b|1\rangle$ and $\omega=e^{i\pi/4}$. After the [controlled-NOT gate](../../../../controlled-not-gate.md), the joint state is

$$
\frac1{\sqrt2}\left[a|0\rangle(|0\rangle+\omega|1\rangle)
+b|1\rangle(\omega|0\rangle+|1\rangle)\right].
$$

An ancilla measurement outcome zero leaves the unnormalized data state $(a|0\rangle+\omega b|1\rangle)/\sqrt2=T|\psi\rangle/\sqrt2$. Outcome one leaves $(\omega a|0\rangle+b|1\rangle)/\sqrt2=\omega T^\dagger|\psi\rangle/\sqrt2$. Both outcomes have [probability](../../../../probability.md) $1/2$. The correction for outcome one is $S$, and $ST^\dagger=T$, so after correction the data is always $T|\psi\rangle$, up to an irrelevant [global phase](../../../../global-phase.md). This proves [magic-state injection of a T gate](../../../../magic-state-injection-of-a-t-gate.md).

The resource state's [Bloch vector](../../../../bloch-vector.md) is $(1/\sqrt2,1/\sqrt2,0)$, outside the [stabilizer octahedron](../../../../stabilizer-octahedron.md). Clifford gates alone preserve stabilizer structure and, with standard-basis preparation and measurement, admit efficient classical simulation by the [Gottesman--Knill theorem](../../../../gottesman-knill-theorem.md). Adding the non-Clifford [T gate](../../../../t-gate.md) supplies a [universal quantum gate set](../../../../universal-quantum-gate-set.md) together with Clifford gates: arbitrary finite-qubit unitaries can be approximated to arbitrary precision. The assertion is approximate universality, not exact representation of every unitary by a finite circuit.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
