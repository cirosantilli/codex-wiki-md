<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $|\alpha\rangle=a|0\rangle+b|1\rangle$ be Alice's unknown qubit, and label her half of the shared [Bell state](../../../../../../bell-state-split.md) by $A$ and Bob's by $B$. Alice applies a [Controlled-NOT gate](../../../../../../controlled-not-gate.md) from the unknown qubit to $A$, then a [Hadamard gate](../../../../../../hadamard-gate.md) to the unknown qubit. The three-qubit state becomes

$$
\frac12\sum_{j,k\in\{0,1\}}|jk\rangle\,X^kZ^j|\alpha\rangle_B.
$$

Alice measures her two qubits in the computational basis and sends the two classical outcomes $(j,k)$ to Bob. Bob applies $Z^jX^k$, recovering $|\alpha\rangle$ with certainty. This is [quantum teleportation](../../../../../../quantum-teleportation.md); Alice never needs to know the state.

For the shared [GHZ state](../../../../../../greenberger-horne-zeilinger-state.md), Charlie first applies a Hadamard gate to his qubit. Then

$$
\frac{|000\rangle+|111\rangle}{\sqrt2}
\longmapsto
\frac1{\sqrt2}\left(|\phi^+\rangle_{AB}|0\rangle_C
+|\phi^-\rangle_{AB}|1\rangle_C\right).
$$

Charlie measures in the computational basis. Outcome $0$ leaves Alice and Bob with $|\phi^+\rangle$; outcome $1$ leaves $|\phi^-\rangle$, which either party converts to $|\phi^+\rangle$ by applying $Z$ after Charlie reports the outcome. Thus

$$
\boxed{\text{Charlie creates the required shared Bell pair with probability one.}}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
