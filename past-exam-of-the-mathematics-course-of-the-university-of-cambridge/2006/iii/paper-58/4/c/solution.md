<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At this stage $A$ is an arbitrary [unitary operator](../../../../../../unitary-operator.md); do not yet assume it prepares the displayed uniform state from zero. Put $|a\rangle=A|0\rangle$, $p=e^{i\phi}$ and $t=e^{i\theta}$. The phase on the zero basis state can be written using a rank-one [orthogonal projection](../../../../../../orthogonal-projection.md) as $S_0^\phi=I+(p-1)|0\rangle\langle0|$, hence

$$
AS_0^\phi A^{-1}=I+(p-1)|a\rangle\langle a|.
$$

The marked-state phase sends $|\psi_1\rangle$ to $t|\psi_1\rangle$ and leaves $|\psi_0\rangle$ unchanged. Therefore

$$
\boxed{Q|\psi_1\rangle=-t\left[|\psi_1\rangle+(p-1)|a\rangle\langle a|\psi_1\rangle\right],}
$$

and

$$
\boxed{Q|\psi_0\rangle=-\left[|\psi_0\rangle+(p-1)|a\rangle\langle a|\psi_0\rangle\right].}
$$

This is the complete general action. Unless $|a\rangle$ lies in their span, that two-dimensional space need not be invariant. The PDF uses $S_f^\theta$ in $Q$; the TeX conversion's replacement by $S_0^\theta$ is a transcription error and would describe a different operation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
