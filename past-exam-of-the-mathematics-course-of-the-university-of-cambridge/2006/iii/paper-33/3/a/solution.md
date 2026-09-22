<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose $|0\rangle$ as the ground state and $|1\rangle$ as the excited state. The relevant [quantum channel](../../../../../../quantum-channel.md) is the [amplitude damping channel](../../../../../../amplitude-damping-channel.md). Its [Kraus operators](../../../../../../kraus-operator.md) are

$$
\boxed{K_0=\begin{pmatrix}1&0\\0&\sqrt{1-p}\end{pmatrix},\qquad K_1=\begin{pmatrix}0&\sqrt p\\0&0\end{pmatrix}=\sqrt p\,|0\rangle\langle1|.}
$$

They satisfy $K_0^\dagger K_0+K_1^\dagger K_1=I$. The $K_0$ branch corresponds to no emitted photon: the ground-state amplitude is unchanged and the excited-state amplitude is attenuated. The $K_1$ branch corresponds to photon emission and transition to the ground state. These are unnormalized branch states; the squared norm or [matrix trace](../../../../../../matrix-trace.md) of each branch gives its probability.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
