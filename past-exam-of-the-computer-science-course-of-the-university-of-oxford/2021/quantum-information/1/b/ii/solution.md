<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Identification is stronger than [quantum state exclusion](../../../../../../quantum-state-exclusion.md). Here an outcome only needs to rule out its associated preparation. Use the following [orthonormal basis](../../../../../../orthonormal-basis.md) for a [basic measurement](../../../../../../basic-measurement.md)

$$
|b_0\rangle=\frac{|0\rangle-|1\rangle}{\sqrt2},\qquad
|b_1\rangle=\frac{|0\rangle+|1\rangle}{\sqrt2},\qquad
|b_2\rangle=|2\rangle.
$$

Its defining overlaps satisfy $\langle b_m|\phi_m\rangle=0$ for $m=0,1,2$. By the [Born rule](../../../../../../born-rule.md), observing $b_m$ makes preparation $\phi_m$ impossible. **Measure in this basis and send its outcome label $m$; the prize is guaranteed.**

For completeness, the [conditional probability](../../../../../../conditional-probability.md) matrix, with rows $m$ and columns the prepared-state label $j$, is

$$
\bigl[\Pr(m\mid\phi_j)\bigr]_{m,j}
=\begin{pmatrix}0&1/2&1/2\\1/2&0&1/2\\1/2&1/2&0\end{pmatrix}.
$$

Every column sums to one and the diagonal vanishes. Each result leaves two possible preparations, so this [projective state exclusion](../../../../../../projective-state-exclusion.md) does not contradict the impossibility of perfect identification. The family consists of [antidistinguishable quantum states](../../../../../../antidistinguishable-quantum-states.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
