<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Phi:M_d(\mathbb C)\to M_D(\mathbb C)$ be a [linear map](../../../../../../linear-map.md). It is [positive](../../../../../../positive-linear-map.md) when $X\geq0$ implies $\Phi(X)\geq0$, and [completely positive](../../../../../../completely-positive-map.md) when

$$
\Phi\otimes\operatorname{id}_r
$$

is positive for every ancillary dimension $r$. In finite dimensions it is enough to check $r=d$.

A finite family of [Kraus operators](../../../../../../kraus-operator.md) $A^\alpha:\mathbb C^d\to\mathbb C^D$ defines the [Kraus representation](../../../../../../kraus-representation.md)

$$
\Phi(X)=\sum_{\alpha=1}^R A^\alpha X(A^\alpha)^\dagger.
$$

This map is completely positive because, for every [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) $Y$ on the enlarged space,

$$
(\Phi\otimes\operatorname{id}_r)(Y)
=\sum_\alpha(A^\alpha\otimes I_r)Y((A^\alpha)^\dagger\otimes I_r)\geq0.
$$

Conversely, use the unnormalized [maximally entangled vector](../../../../../../maximally-entangled-state.md) $|\Omega\rangle=\sum_{j=1}^d|j\rangle|j\rangle$. Complete positivity makes the [Choi matrix](../../../../../../choi-matrix.md)

$$
C_\Phi=(\Phi\otimes\operatorname{id}_d)(|\Omega\rangle\langle\Omega|)
$$

positive semidefinite. By the [spectral theorem for normal operators](../../../../../../spectral-theorem-for-normal-operators.md), $C_\Phi=\sum_{\alpha=1}^R|v_\alpha\rangle\langle v_\alpha|$, where $R=\operatorname{rank}C_\Phi\leq dD$. Reshape each $v_\alpha\in\mathbb C^D\otimes\mathbb C^d$ into a matrix $A^\alpha$ by $|v_\alpha\rangle=\sum_{\mu j}A^\alpha_{\mu j}|\mu\rangle|j\rangle$. The [Choi matrix](../../../../../../choi-matrix.md) inversion formula

$$
\Phi(X)=\operatorname{Tr}_{\rm in}\!\left[C_\Phi(I_D\otimes X^T)\right]
$$

then gives $\Phi(X)=\sum_\alpha A^\alpha X(A^\alpha)^\dagger$. Thus finite [Kraus representations](../../../../../../kraus-representation.md) characterize finite-dimensional completely positive maps.

The additional normalization

$$
\sum_\alpha(A^\alpha)^\dagger A^\alpha=I_d
$$

makes $\Phi$ trace preserving and hence a [quantum channel](../../../../../../quantum-channel.md); $\sum_\alpha A^\alpha(A^\alpha)^\dagger=I_D$ instead makes it unital.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
