<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $x_i=\langle\psi_i|X|\psi_i\rangle$, which is real because $X$ is a [Hermitian operator](../../../../../../hermitian-operator.md). Set

$$
T=\sum_i\operatorname{sgn}(x_i)|\psi_i\rangle\langle\psi_i|,
$$

with $\operatorname{sgn}(0)=0$. This [Hermitian operator](../../../../../../hermitian-operator.md) satisfies $-I\leq T\leq I$. The [trace-norm variational principle for Hermitian operators](../../../../../../trace-norm-variational-principle-for-hermitian-operators.md) gives the [diagonal absolute-sum bound for the trace norm](../../../../../../diagonal-absolute-sum-bound-for-the-trace-norm.md):

$$
\boxed{\|X\|_1\geq\operatorname{Tr}(XT)=\sum_i|\langle\psi_i|X|\psi_i\rangle|.}
$$

For $X=\rho-P$, with $P=|\psi\rangle\langle\psi|$, extend $|\psi\rangle$ to an [orthonormal basis](../../../../../../orthonormal-basis.md) $|\psi_1\rangle=|\psi\rangle,|\psi_2\rangle,\ldots$. Put $r=\langle\psi|\rho|\psi\rangle$. The first diagonal entry is $r-1\leq0$, and all the others are nonnegative. Their sum is $1-r$, because $\operatorname{Tr}\rho=1$. The bound therefore yields $\|\rho-P\|_1\geq2(1-r)$. Using the definitions of [trace distance](../../../../../../trace-distance.md) and [quantum fidelity](../../../../../../fidelity-of-quantum-states.md),

$$
\boxed{D(\rho,P)\geq1-r=1-F(\rho,P)^2.}
$$

This [pure-target lower bound on trace distance](../../../../../../pure-target-lower-bound-on-trace-distance.md) is attained whenever $\rho$ has no coherence between $|\psi\rangle$ and its orthogonal complement. The proof used the [trace-norm variational principle for Hermitian operators](../../../../../../trace-norm-variational-principle-for-hermitian-operators.md), together with positivity and normalization of a [density operator](../../../../../../density-matrix.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
