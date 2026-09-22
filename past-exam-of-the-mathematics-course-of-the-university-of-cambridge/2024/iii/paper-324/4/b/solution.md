<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [HHL algorithm](../../../../../../hhl-algorithm.md) requires coherent, efficient and repeatable preparation of the normalized state $|b\rangle$, normally through a known preparation circuit and its inverse; possession of a single unknown physical specimen does not supply that access. The component of $b$ on any discarded or unresolved small-eigenvalue subspace must also be negligible. Here $U$ is a [unitary operator](../../../../../../unitary-operator.md), so it is invertible and all its [singular values](../../../../../../singular-value.md) equal one, giving [condition number](../../../../../../condition-number.md) $\kappa=1$.

Standard HHL is stated for a [Hermitian matrix](../../../../../../hermitian-operator.md) with an efficient sparse-access or [block encoding](../../../../../../block-encoding.md) oracle. A non-Hermitian $U$ can be embedded in the Hermitian block matrix

$$
\begin{pmatrix}0&U\\U^\dagger&0\end{pmatrix};
$$

part (a) supplies efficient access to $U^\dagger$. With inverse-polynomial target precision, $m=O(\log n)$ phase bits, and an efficient preparation oracle for $|b\rangle$, the runtime is $\operatorname{poly}(n)$. The output is the normalized [quantum state](../../../../../../quantum-state.md) proportional to the solution $x$, rather than a classical list of all its amplitudes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
