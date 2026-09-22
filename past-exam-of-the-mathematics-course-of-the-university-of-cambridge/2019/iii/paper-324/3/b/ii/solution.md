<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since $A|x\rangle=(-1)^{f(x)}|x\rangle$, the [spectral decomposition](../../../../../../../spectral-decomposition.md) gives

$$
e^{iA}|x\rangle=e^{i(-1)^{f(x)}}|x\rangle.
$$

Replace the middle gate of the previous [compute-phase-uncompute construction](../../../../../../../compute-phase-uncompute-construction.md) by

$$
e^{iZ}=\operatorname{diag}(e^i,e^{-i})=R_z(-2),
$$

a one-qubit [rotation about the z-axis](../../../../../../../rotation-about-the-z-axis.md). Then

$$
\boxed{C^\dagger(I\otimes e^{iZ})C\,|x,0\rangle
=e^{i(-1)^{f(x)}}|x,0\rangle.}
$$

The circuit uses the gates of $C$, their inverses, and one fixed rotation; it returns the [quantum ancilla](../../../../../../../quantum-ancilla.md) to $|0\rangle$. The same construction implements $e^{itA}$ with middle gate $e^{itZ}$, an instance of [simulation of a computable diagonal Hamiltonian](../../../../../../../simulation-of-a-computable-diagonal-hamiltonian.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
