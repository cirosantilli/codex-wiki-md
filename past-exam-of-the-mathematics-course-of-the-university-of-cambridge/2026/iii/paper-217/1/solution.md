<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Because $V$ is measurable for the [cylinder sigma-algebra](../../../../../cylinder-sigma-algebra.md), membership in $V$ depends on only countably many coordinates $T_0=\{t_1,t_2,\ldots\}$. Its image in $\mathbb R^{T_0}$ is a measurable linear subspace $V_0$, and

$$
\{X\in V\}=\{(X(t_j))_{j\geq1}\in V_0\}.
$$

By successively applying the finite-dimensional Gaussian regression formula, realize this Gaussian sequence as a lower-triangular linear transform of independent standard normal variables:

$$
(X(t_j))_{j\geq1}=\sum_{k\geq1}g_k a_k,
$$

where every coordinate of the sum contains only finitely many terms. If some deterministic column $a_k$ does not belong to $V_0$, then, after conditioning on every $g_j$ except $g_k$, at most one value of $g_k$ can put the sum in $V_0$. The continuous normal distribution gives probability zero. If every $a_k$ belongs to $V_0$, changing finitely many $g_k$ does not change the membership event. It is then a [tail event](../../../../../tail-event.md), and the [Kolmogorov zero-one law](../../../../../kolmogorov-s-zero-one-law.md) gives probability zero or one. This proves the [Gaussian zero-one law for measurable linear subspaces](../../../../../gaussian-zero-one-law-for-measurable-linear-subspaces.md).

Now let $X(t)=\sqrt t,g_t$ for independent standard normal variables $g_t$. Define

$$
V=\left\{x\in\mathbb R^{\mathbb N}:\frac{x_t}{t}\longrightarrow0\right\},
\qquad
W=\ell^2.
$$

Both are cylinder-measurable infinite-dimensional linear subspaces. For every $\varepsilon>0$,

$$
\sum_{t=1}^\infty\mathbb P(|g_t|>\varepsilon\sqrt t)<\infty,
$$

so the [Borel-Cantelli lemmas](../../../../../borel-cantelli-lemmas.md) imply $g_t/\sqrt t\to0$ almost surely and hence $\mathbb P(X\in V)=1$. On the other hand, $g_t^2\geq1$ infinitely often almost surely, again by Borel-Cantelli, so

$$
\sum_{t=1}^\infty|X(t)|^2=\sum_{t=1}^\infty t g_t^2=\infty
$$

almost surely. Therefore $\mathbb P(X\in W)=0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
