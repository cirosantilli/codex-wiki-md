<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a [Clifford operation](../../../../../../../clifford-gate.md) $D$ with $D|0^n\rangle=|\sigma\rangle$ and absorb $D$ into the circuit. Push each subsequent Clifford gate forward through the computation. A computational-basis measurement made after a Clifford prefix $U$ becomes a [Pauli measurement](../../../../../../../measurement-of-a-pauli-observable.md)

$$
Z_j\longmapsto U^\dagger Z_jU
$$

on the initial state, because Clifford conjugation preserves the [Pauli group](../../../../../../../pauli-group.md). Adaptivity merely makes the next Pauli depend on earlier classical outcomes.

It remains to eliminate the $n$ stabilizer qubits. Maintain their current [stabilizer group](../../../../../../../stabilizer-group.md). For a Pauli $P$ to be measured, there are two cases.


- If $P$ commutes with every stabilizer generator, its action on the one-dimensional stabilizer sector reduces to a Pauli operator on the remaining $t$ qubits, possibly with a known sign. Measure that effective Pauli on $|\rho\rangle$.
- If $P$ anticommutes with some stabilizer $S$, its outcome $\lambda\in\{+1,-1\}$ is uniformly random. Sample $\lambda$ for an ordinary measurement, or set $\lambda=+1$ when the original measurement is postselected. The Clifford operator


$$
V_\lambda=\frac{I+\lambda PS}{\sqrt2}
$$

maps the old stabilizer sector into the $\lambda$ eigenspace of $P$. Updating the Clifford frame by $V_\lambda$ removes this measurement while conjugating every later Pauli to another Pauli.

Iterating this procedure leaves an adaptive [Pauli-based computation](../../../../../../../pauli-based-computation.md) on $|\rho\rangle$. The same classical outcomes determine every adaptive choice and final output, so this gives a [weak classical simulation](../../../../../../../weak-classical-simulation-of-a-quantum-circuit.md). Every postselected $Z$ outcome becomes either a fixed classical $+1$ branch or a postselected $+1$ Pauli measurement, as required.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
