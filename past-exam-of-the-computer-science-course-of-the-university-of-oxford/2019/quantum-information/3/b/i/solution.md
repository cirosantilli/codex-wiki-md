<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Both the [controlled-NOT gate](../../../../../../controlled-not-gate.md) and [Pauli X gate](../../../../../../pauli-x-gate.md) permute [computational basis](../../../../../../computational-basis.md) [vectors](../../../../../../vector.md). Any finite composition remains a [permutation matrix](../../../../../../permutation-matrix.md), and so sends $|0\cdots0\rangle$ to another [computational basis](../../../../../../computational-basis.md) [vector](../../../../../../vector.md). It cannot prepare a superposition such as $|+\rangle\otimes|0\cdots0\rangle$.

This also rules out approximation: the squared overlap of that target with any [computational basis](../../../../../../computational-basis.md) [vector](../../../../../../vector.md) is at most $1/2$, so even after optimizing [global phase](../../../../../../global-phase.md) the [pure-state norm distance](../../../../../../pure-state-norm-distance.md) is at least $\sqrt{2-\sqrt2}>0$. Hence **$\{CNOT,X\}$ is not universal**. Basis permutations can create entanglement on some superposed inputs, but this gate set cannot create the required superposition from the specified basis input.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
