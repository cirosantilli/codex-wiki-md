<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use base-two logarithms for [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md), so the units are [bits](../../../../../../bit.md), and adopt $0\log_2 0=0$. All systems here may be taken finite-dimensional; the entropy arguments also apply when the displayed [Von Neumann entropies](../../../../../../von-neumann-entropy-split.md) are finite. The [density operator](../../../../../../density-matrix.md) of the joint [pure state](../../../../../../pure-state.md) is $\rho_{AB}=|\Psi_{AB}\rangle\langle\Psi_{AB}|$. It is a rank-one [orthogonal projector](../../../../../../orthogonal-projection.md), whose only nonzero [eigenvalue](../../../../../../eigenvalue.md) is one. Consequently

$$
\boxed{S(A,B)=-\operatorname{Tr}(\rho_{AB}\log_2\rho_{AB})=0.}
$$

The [reduced density matrices](../../../../../../reduced-density-matrix.md) are $\rho_A=\operatorname{Tr}_B\rho_{AB}$ and $\rho_B=\operatorname{Tr}_A\rho_{AB}$. The [quantum conditional entropy](../../../../../../quantum-conditional-entropy.md) is defined by the entropy difference

$$
S(B|A):=S(\rho_{AB})-S(\rho_A).
$$

For the [pure state](../../../../../../pure-state.md) under consideration this becomes $S(B|A)=-S(\rho_A)$. To determine when it is negative, write the [Schmidt decomposition](../../../../../../schmidt-decomposition.md)

$$
|\Psi_{AB}\rangle=\sum_{j=1}^r\sqrt{\lambda_j}|a_j\rangle|b_j\rangle,
\qquad \lambda_j>0,\qquad\sum_j\lambda_j=1.
$$

The [eigenvalues](../../../../../../eigenvalue.md) of $\rho_A$ are the $\lambda_j$, together with possible zeros. Each contribution $-\lambda_j\log_2\lambda_j$ is nonnegative, and their sum vanishes exactly when one [eigenvalue](../../../../../../eigenvalue.md) equals one. Equivalently the [Schmidt rank](../../../../../../schmidt-rank.md) is one and $|\Psi_{AB}\rangle$ is a [product state](../../../../../../product-state.md). If the [pure state](../../../../../../pure-state.md) is [entangled](../../../../../../entangled-state.md), then $r\geq2$, every nonzero [eigenvalue](../../../../../../eigenvalue.md) is strictly below one, and the [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is strictly positive. Thus the [pure-state negative conditional entropy criterion](../../../../../../pure-state-negative-conditional-entropy-criterion.md) gives

$$
\boxed{S(B|A)<0\quad\Longleftrightarrow\quad|\Psi_{AB}\rangle\text{ is entangled}.}
$$

The purity assumption matters: for mixed [density operators](../../../../../../density-matrix.md), negative [quantum conditional entropy](../../../../../../quantum-conditional-entropy.md) is not necessary for [entanglement](../../../../../../entangled-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
