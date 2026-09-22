<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose independent random variables $\xi_i\sim N(0,1)$ on a countable product probability space. For each fixed $t$, the diagonal assumption gives

$$
\sum_i k_i(t)^2=K(t,t)<\infty.
$$

The partial sums $\sum_{i\leq n}k_i(t)\xi_i$ are therefore Cauchy in $L^2$. Define

$$
\boxed{X_t=L^2\text{-}\lim_{n\to\infty}\sum_{i=1}^n k_i(t)\xi_i.}
$$

Choose a representative of this limit for each $t$. No path continuity or simultaneous series convergence over all uncountably many times is being asserted.

For any finite list $t_1,\ldots,t_m$ and real coefficients $a_j$, the linear combination $\sum_ja_jX_{t_j}$ is the $L^2$ limit of centered Gaussian variables

$$
\sum_{i=1}^n\left(\sum_{j=1}^m a_jk_i(t_j)\right)\xi_i.
$$

Their variances converge, so their [characteristic functions](../../../../../../characteristic-function.md) converge to that of a centered [normal distribution](../../../../../../normal-distribution.md). This proves that every finite-dimensional vector is Gaussian and hence that $X$ is a [Gaussian process](../../../../../../gaussian-process.md). Taking $L^2$ limits also gives

$$
\boxed{\mathbb EX_t=0,\qquad
\mathbb E[X_sX_t]=\sum_i k_i(s)k_i(t)=K(s,t).}
$$

This is the [Gaussian process construction from square-summable features](../../../../../../gaussian-process-construction-from-square-summable-features.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
