<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because the scalar signal and the noise vector are [independent random variables](../../../../../../independent-random-variables.md) with [normal distributions](../../../../../../normal-distribution.md), their sum is a [Gaussian random vector](../../../../../../gaussian-random-vector.md). Its [expected value](../../../../../../expected-value.md) is zero, and the [covariance matrix](../../../../../../covariance-matrix.md) is

$$
\boxed{\Sigma_S=I_d+\theta u(S)u(S)^\top,\qquad P_{\theta,S}=N(0,\Sigma_S).}
$$

Thus this is a [rank-one covariance spike](../../../../../../rank-one-covariance-spike.md). Each summand $X_iX_i^\top$ has [expected value](../../../../../../expected-value.md) $\Sigma_S$, so **$\mathbb E\widehat\Sigma=\Sigma_S$**. Here the empirical matrix is an [uncentered empirical second-moment matrix](../../../../../../uncentered-empirical-second-moment-matrix.md); because the population [expected value](../../../../../../expected-value.md) is known to be zero, it is an [unbiased estimator](../../../../../../unbiased-estimator.md) of the [covariance matrix](../../../../../../covariance-matrix.md). The TeX's apparent factorial denominator is a transcription error.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
