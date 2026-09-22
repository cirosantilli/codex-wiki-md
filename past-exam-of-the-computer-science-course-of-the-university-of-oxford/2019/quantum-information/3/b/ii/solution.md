<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Squaring the diagonal gate gives

$$
V^2=\operatorname{diag}(e^{-i\pi/8},e^{i\pi/8})=e^{-i\pi/8}T.
$$

Thus the [T gate](../../../../../../t-gate.md) is available up to a [global phase](../../../../../../global-phase.md). Reading the supplied W columns in order $00,01,10,11$, it sends $|01\rangle$ to $|11\rangle$, $|11\rangle$ to $|01\rangle$, and fixes the other two [vectors](../../../../../../vector.md): it is CNOT with the _second_ wire controlling the first. Conjugating both wires by the [Hadamard gate](../../../../../../hadamard-gate.md) reverses that orientation:

$$
\boxed{\mathrm{CNOT}_{1\to2}=(H\otimes H)W(H\otimes H).}
$$

For instance, write $W=I\otimes|0\rangle\langle0|+X\otimes|1\rangle\langle1|$. Conjugation uses $HXH=Z$ and $H|0\rangle=|+\rangle$, $H|1\rangle=|-\rangle$, yielding $I\otimes|+\rangle\langle+|+Z\otimes|-\rangle\langle-|$. Expanding the first-wire Z eigenspaces gives $|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes X$, as required.

We have H directly and finite constructions of CNOT and T up to physically irrelevant [global phase](../../../../../../global-phase.md). By [universality transfer by exact gate synthesis](../../../../../../universality-transfer-by-exact-gate-synthesis.md), the assumed universality of $\{CNOT,H,T\}$ proves that **$\{V,H,W\}$ is universal under the phase-insensitive convention**. There is no assertion of arbitrary strict operator-norm phases: on a fixed register these generators have only a [finite set](../../../../../../finite-set.md) of possible determinants, which would obstruct density in the entire unitary group if [global phase](../../../../../../global-phase.md) were treated as an observable target.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
