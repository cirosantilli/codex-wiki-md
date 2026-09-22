<h1 id="2/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a [singular system of a compact operator](../../../../../../../singular-system-of-a-compact-operator.md), with $Kv_j=\sigma_jw_j$ and $K^*w_j=\sigma_jv_j$, $\sigma_j>0$. A [spectral regularization method](../../../../../../../spectral-regularization-method.md) has the form

$$
\boxed{R_\alpha f=\sum_j\sigma_jg_\alpha(\sigma_j^2)
\langle f,w_j\rangle v_j.}
$$

It annihilates $\mathcal R(K)^\perp$. Standard sufficient [spectral filter](../../../../../../../spectral-filter.md) conditions are boundedness of $\sup_{0<\sigma\leq\|K\|}|\sigma g_\alpha(\sigma^2)|$ for each $\alpha$, pointwise $\lambda g_\alpha(\lambda)\to1$ as $\alpha\downarrow0$ for $\lambda>0$, and a uniform bound on $|\lambda g_\alpha(\lambda)|$. These give bounded linear operators and convergence on the domain of the [Moore–Penrose inverse of an operator](../../../../../../../moore-penrose-inverse-of-an-operator.md) by the [Picard criterion](../../../../../../../picard-criterion.md) and [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md).

For [Tikhonov regularization](../../../../../../../tikhonov-regularization.md),

$$
g_\alpha(\lambda)=\frac1{\lambda+\alpha},\qquad
\boxed{R_\alpha=(K^*K+\alpha I)^{-1}K^*.}
$$

This can be computed by solving the [Tikhonov normal equation](../../../../../../../tikhonov-normal-equation.md), without knowing the [singular value decomposition](../../../../../../../singular-value-decomposition.md).

For [spectral cutoff regularization](../../../../../../../truncated-singular-value-decomposition.md), take

$$
\boxed{g_\alpha(\lambda)=\frac{\mathbf1_{[\alpha,\infty)}(\lambda)}{\lambda},}
$$

with value zero at $\lambda=0$. Only [singular values](../../../../../../../singular-value.md) $\sigma_j\geq\sqrt\alpha$ are inverted. Here $g_\alpha$ multiplies $\sigma$; conventions calling the full coefficient $\sigma g_\alpha(\sigma^2)$ the [spectral filter](../../../../../../../spectral-filter.md) are equivalent.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
