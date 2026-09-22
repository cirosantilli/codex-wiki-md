<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md) changes only the amplitude of $|x_0\rangle$. Since that amplitude in $|\psi\rangle$ is $1/2$,

$$
\boxed{I_{x_0}|\psi\rangle=|\psi\rangle-|x_0\rangle.}
$$

Also,

$$
\boxed{|\psi\rangle\langle\psi|x_0\rangle=\frac12|\psi\rangle.}
$$

It follows that $A|\psi\rangle=-|\psi\rangle$ and $A|x_0\rangle=|x_0\rangle-|\psi\rangle$, so

$$
A I_{x_0}|\psi\rangle
=A(|\psi\rangle-|x_0\rangle)
=-|x_0\rangle.
$$

The global minus sign has no observable effect. Prepare $|\psi\rangle=H^{\otimes2}|00\rangle$, query $I_{x_0}$ once, apply the fixed operator $A$, and perform a [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md). The outcome is $x_0$ with probability one. This is [exact Grover search on four entries](../../../../../../exact-grover-search-on-four-entries.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
