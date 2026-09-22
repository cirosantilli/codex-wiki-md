<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The useful object is the [Choi state](../../../../../../choi-state.md) of the [entanglement-breaking channel](../../../../../../entanglement-breaking-channel.md). Put $d_A=\dim\mathcal H_A$, introduce a reference $R$ with the same [computational basis](../../../../../../computational-basis.md) as $A$, and use the normalized [maximally entangled state](../../../../../../maximally-entangled-state.md)

$$
|\Phi\rangle_{RA}=d_A^{-1/2}\sum_j|j\rangle_R|j\rangle_A,\qquad
C_{RB}=(\operatorname{id}_R\otimes\mathcal E)(|\Phi\rangle\langle\Phi|).
$$

The [entanglement-breaking channel](../../../../../../entanglement-breaking-channel.md) makes $C_{RB}$ a [separable quantum state](../../../../../../separable-quantum-state.md). Its [partial trace](../../../../../../partial-trace.md) is $\operatorname{Tr}_B C_{RB}=I_R/d_A$, because $\mathcal E$ is a [quantum channel](../../../../../../quantum-channel.md). Write a [separable positive operator](../../../../../../separable-positive-operator.md) decomposition

$$
C_{RB}=\sum_y\alpha_y\otimes\beta_y,\qquad \alpha_y\geq0,\quad\beta_y\geq0.
$$

Discard any term with $\operatorname{Tr}\beta_y=0$: a [positive operator](../../../../../../positive-operator.md) with zero [trace](../../../../../../matrix-trace.md) is zero. Define

$$
\tau_y=\frac{\beta_y}{\operatorname{Tr}\beta_y},\qquad
E_y=d_A(\operatorname{Tr}\beta_y)\alpha_y^T.
$$

Each $\tau_y$ is a [density operator](../../../../../../density-matrix.md). Each $E_y$ is a [positive operator](../../../../../../positive-operator.md), and taking the [matrix transpose](../../../../../../transpose.md) of the [partial trace](../../../../../../partial-trace.md) identity gives

$$
\sum_y E_y=d_A\left(\sum_y(\operatorname{Tr}\beta_y)\alpha_y\right)^T=I_A.
$$

Thus the $E_y$ form a [POVM](../../../../../../positive-operator-valued-measure.md). In this reference-first convention, the [Choi reconstruction formula](../../../../../../choi-reconstruction-formula.md) is

$$
\mathcal E(L)=d_A\operatorname{Tr}_R[(L^T\otimes I_B)C_{RB}]
=\sum_y\tau_y\operatorname{Tr}(E_yL).
$$

The factor $d_A$ is essential because we used a normalized [Choi state](../../../../../../choi-state.md). A [measurement channel](../../../../../../measurement-channel.md) storing the outcome $y$, followed by the prescribed [quantum state preparation](../../../../../../quantum-state-preparation.md) of $\tau_y$, has precisely this action on every [linear operator](../../../../../../linear-operator.md) $L$. **The desired factorization is therefore**

$$
\boxed{\mathcal E^{B\leftarrow A}=\mathcal P^{B\leftarrow\widetilde Y}\mathcal M^{\widetilde Y\leftarrow A}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
