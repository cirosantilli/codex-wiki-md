<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work with a nonsingular [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), so $V$ is [positive-definite](../../../../../../positive-definite-bilinear-form.md). The claimed finite [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) also require the centered [sample covariance matrix](../../../../../../sample-covariance-matrix.md) to be nonsingular; the exceptional case is discussed below.

Independence gives, up to a constant, the [log-likelihood](../../../../../../log-likelihood.md)

$$
\ell(\mu,V)=-\frac n2\log\det V
-\frac12\sum_{i=1}^n(Y_i-\mu)^TV^{-1}(Y_i-\mu).
$$

Let $\bar Y=n^{-1}\sum_iY_i$ and $S=n^{-1}\sum_i(Y_i-\bar Y)(Y_i-\bar Y)^T$. The centered sum is zero, and expansion therefore gives

$$
\sum_i(Y_i-\mu)(Y_i-\mu)^T
=nS+n(\bar Y-\mu)(\bar Y-\mu)^T.
$$

For every fixed [positive-definite matrix](../../../../../../positive-definite-matrix.md) $V$, the extra quadratic term in the [log-likelihood](../../../../../../log-likelihood.md) is $-n(\bar Y-\mu)^TV^{-1}(\bar Y-\mu)/2$, with unique maximum at $\mu=\bar Y$.

Assume $S$ is [positive-definite](../../../../../../positive-definite-bilinear-form.md). Maximizing over $V$ now means minimizing $\log\det V+\operatorname{tr}(V^{-1}S)$. Put $A=S^{1/2}V^{-1}S^{1/2}$, another [positive-definite matrix](../../../../../../positive-definite-matrix.md). Then

$$
\log\det V+\operatorname{tr}(V^{-1}S)
=\log\det S-\log\det A+\operatorname{tr}A.
$$

If $a_1,\ldots,a_p>0$ are its [eigenvalues](../../../../../../eigenvalue.md), the variable part is $\sum_j(a_j-\log a_j)$. The scalar inequality $a-\log a\ge1$, with equality only at $a=1$, shows that this is minimized uniquely at $A=I$, or $V=S$. Thus

$$
\boxed{\widehat\mu=\bar Y,\qquad
\widehat V=S=\frac1n\sum_i(Y_i-\bar Y)(Y_i-\bar Y)^T.}
$$

The divisor is $n$ because this is [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md), not the unbiased [covariance](../../../../../../covariance.md) estimate with divisor $n-1$.

The nonsingularity condition matters. The centered scatter has [rank](../../../../../../rank-one-quadratic-form.md) at most $n-1$. If $S$ is singular, choose $\mu=\bar Y$, retain positive [covariance](../../../../../../covariance.md) [eigenvalues](../../../../../../eigenvalue.md) on its range and let a [covariance](../../../../../../covariance.md) [eigenvalue](../../../../../../eigenvalue.md) on its [null space](../../../../../../kernel-of-a-linear-map.md) tend to zero. The quadratic [likelihood](../../../../../../likelihood-function.md) term remains finite, while $-\log\det V\to+\infty$. This is [singular covariance and nonexistence of a Gaussian maximum likelihood estimate](../../../../../../singular-covariance-and-nonexistence-of-a-gaussian-maximum-likelihood-estimate.md): there is no finite maximizer over nonsingular $V$. Under a nonsingular [Gaussian](../../../../../../normal-distribution.md) population, $S$ is positive definite almost surely when $n>p$; for $n\le p$ it is necessarily singular. The asserted estimate and the inverse in the next part have their usual meaning under $n>p$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
