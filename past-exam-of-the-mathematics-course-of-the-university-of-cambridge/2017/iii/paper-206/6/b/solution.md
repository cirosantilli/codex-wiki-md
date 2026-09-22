<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $z=(Z_{s_1},\ldots,Z_{s_n})^T$, let $\Sigma_{ij}=C(\|s_i-s_j\|)$, let $c_i=C(\|s_i-s_0\|)$, and put $v_0=C(0)$. Assume the [covariance matrix](../../../../../../covariance-matrix.md) $\Sigma$ is invertible. Because the mean is known to be zero, every linear predictor $w^Tz$ is unbiased. Its [mean squared prediction error](../../../../../../mean-squared-prediction-error.md) is

$$
\mathbb E(Z_{s_0}-w^Tz)^2=v_0-2w^Tc+w^T\Sigma w.
$$

Completing the square yields

$$
v_0-c^T\Sigma^{-1}c+(w-\Sigma^{-1}c)^T\Sigma(w-\Sigma^{-1}c).
$$

The [positive-definite matrix](../../../../../../positive-definite-matrix.md) property makes the last term nonnegative, proving the [simple kriging](../../../../../../simple-kriging.md) formulas

$$
\boxed{\widehat Z_{s_0}=c^T\Sigma^{-1}z,\qquad v_K=v_0-c^T\Sigma^{-1}c.}
$$

The residual is uncorrelated with $z$. Since the joint law is [multivariate normal](../../../../../../multivariate-normal-distribution.md), it is independent of $z$, so the same predictor and [variance](../../../../../../variance-split.md) describe the [conditional distribution](../../../../../../conditional-distribution.md). Consequently a 95-percent [prediction interval](../../../../../../prediction-interval.md) is

$$
\boxed{c^T\Sigma^{-1}z\ \pm\ q_{0.025}\sqrt{v_0-c^T\Sigma^{-1}c}.}
$$

There is no constraint that the weights sum to one: that is required for an unknown constant mean in [ordinary kriging](../../../../../../ordinary-kriging.md), not for the stated known-zero-mean problem. If $\Sigma$ is singular, use a [Moore-Penrose inverse](../../../../../../moore-penrose-inverse.md) with the corresponding [covariance](../../../../../../covariance.md) compatibility condition. At an already observed location prediction of that very same field value has zero error; predicting an independent noisy replicate is a different target. Estimated [covariance](../../../../../../covariance.md) parameters make this a plug-in interval and generally add uncertainty that the formula does not include.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
