<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label the atomic ground state $|0\rangle$ and excited state $|1\rangle$, with $0\leq p\leq1$. The process is the [amplitude damping channel](../../../../../../amplitude-damping-channel.md), with [Kraus operators](../../../../../../kraus-operator.md)

$$
\boxed{A_0=|0\rangle\langle0|+\sqrt{1-p}\,|1\rangle\langle1|
=\begin{pmatrix}1&0\\0&\sqrt{1-p}\end{pmatrix},
\qquad
A_1=\sqrt p\,|0\rangle\langle1|
=\begin{pmatrix}0&\sqrt p\\0&0\end{pmatrix}.}
$$

They satisfy $A_0^\dagger A_0+A_1^\dagger A_1=I$, so the resulting [Kraus representation](../../../../../../kraus-representation.md) is [trace](../../../../../../matrix-trace.md) preserving.

The operator $A_1$ represents emission: it maps the excited state to $\sqrt p$ times the ground state and annihilates the ground state. Its probability for an initially excited atom is $p$. The operator $A_0$ represents no emission: it leaves the ground state unchanged and retains the excited amplitude with factor $\sqrt{1-p}$. This branch is not generally the identity operation; the absence of a photon itself changes the conditional relative amplitudes. For an arbitrary atomic [density operator](../../../../../../density-matrix.md), the emission probability is $\operatorname{Tr}(A_1\rho A_1^\dagger)=p\rho_{11}$ and the no-emission probability is $1-p\rho_{11}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
