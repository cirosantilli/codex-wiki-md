<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the vectors in the [quantum state ensemble](../../../../../../quantum-state-ensemble.md) to be normalized, with $p_i\geq0$ and $\sum_i p_i=1$. The corresponding [density matrix](../../../../../../density-matrix.md) is

$$
\boxed{\rho=\sum_i p_i|\psi_i\rangle\langle\psi_i|.}
$$

Each rank-one projector is a [self-adjoint operator](../../../../../../self-adjoint-operator.md), so $\rho^\dagger=\rho$. For every $|v\rangle$ in the [Hilbert space](../../../../../../hilbert-space-split.md),

$$
\langle v|\rho|v\rangle=\sum_i p_i|\langle\psi_i|v\rangle|^2\geq0,
$$

proving that $\rho$ is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md). The [trace](../../../../../../matrix-trace.md) is $\operatorname{Tr}\rho=\sum_i p_i\langle\psi_i|\psi_i\rangle=1$.

Conversely, diagonalize a [self-adjoint operator](../../../../../../self-adjoint-operator.md) $\rho$ in an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md), writing $\rho=\sum_j\lambda_j|e_j\rangle\langle e_j|$. Its [positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md) implies $\lambda_j=\langle e_j|\rho|e_j\rangle\geq0$, and its unit [trace](../../../../../../matrix-trace.md) gives $\sum_j\lambda_j=1$. Thus $\{\lambda_j,|e_j\rangle\}$ is a [quantum state ensemble](../../../../../../quantum-state-ensemble.md) with precisely this [density matrix](../../../../../../density-matrix.md). Terms with zero [eigenvalue](../../../../../../eigenvalue.md) may be omitted. This argument includes rank-one [pure states](../../../../../../pure-state.md); an ensemble representation need not describe a genuinely [mixed state](../../../../../../mixed-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
