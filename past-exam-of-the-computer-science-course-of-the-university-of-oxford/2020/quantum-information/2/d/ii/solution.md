<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $S=\operatorname{diag}(1,i)=T^2$ and the [Pauli X gate](../../../../../../pauli-x-gate.md). Starting with the [Bell state](../../../../../../bell-state-split.md) $|\Phi^+\rangle$, the exact constructions are

$$
\boxed{|\Psi_1\rangle=(S\otimes X)|\Phi^+\rangle,\qquad |\Psi_2\rangle=(I\otimes H)|\Phi^+\rangle.}
$$

For the first, $I\otimes X$ changes the two terms to $|01\rangle$ and $|10\rangle$, and $S\otimes I$ multiplies just the second term by $i$. For the second,

$$
(I\otimes H)|\Phi^+\rangle=\frac{|0\rangle|+\rangle+|1\rangle|-\rangle}{\sqrt2}=\frac{|00\rangle+|01\rangle+|10\rangle-|11\rangle}{2}.
$$

All factors are single-party [unitary operators](../../../../../../unitary-operator.md), proving both claimed [local-unitary equivalences](../../../../../../local-unitary-equivalence.md). The equations hold as [vectors](../../../../../../vector.md), without even an additional [global phase](../../../../../../global-phase.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
