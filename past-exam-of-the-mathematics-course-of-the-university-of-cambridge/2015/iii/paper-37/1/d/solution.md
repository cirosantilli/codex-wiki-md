<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By the [causality root criterion for an autoregressive model](../../../../../../causality-root-criterion-for-an-autoregressive-model.md), choose $r>1$ smaller than the modulus of every root of $\Phi$. The function $\Psi=1/\Phi$ is an [analytic function](../../../../../../space-of-holomorphic-functions.md) on and inside $|z|=r$. Writing $M=\max_{|z|=r}|1/\Phi(z)|$, the [Cauchy estimate](../../../../../../cauchy-estimate.md) gives $|\psi_j|\leq Mr^{-j}$. For $h\geq0$, [independence](../../../../../../independent-random-variables.md) of the noise in the [infinite moving-average representation](../../../../../../infinite-moving-average-representation.md) gives

$$
\gamma(h)=\sigma^2\sum_{j\geq0}\psi_j\psi_{j+h},\qquad
|\gamma(h)|\leq\frac{\sigma^2M^2}{1-r^{-2}}r^{-h}.
$$

The [autocovariance](../../../../../../autocovariance.md) is symmetric in the lag. Thus **exponential decay holds** with

$$
\boxed{s=r^{-1}\in(0,1),\qquad C=\frac{\sigma^2M^2}{1-r^{-2}}.}
$$

This is [exponential autocovariance decay of a causal autoregression](../../../../../../exponential-autocovariance-decay-of-a-causal-autoregression.md). If $\Phi$ is constant, there are no roots and any $r>1$ works.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
