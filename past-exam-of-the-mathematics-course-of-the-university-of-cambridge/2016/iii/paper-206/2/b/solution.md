<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [fitted values](../../../../../../fitted-values.md) are $\widehat Y=X\widehat\beta$, so the [hat matrix](../../../../../../hat-matrix.md) is

$$
\boxed{H=X(X^TX)^{-1}X^T.}
$$

It is symmetric, and

$$
H^2=X(X^TX)^{-1}(X^TX)(X^TX)^{-1}X^T=H.
$$

It fixes every vector in the column space of $X$, and annihilates its orthogonal complement. Thus $H$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto that column space, has [matrix rank](../../../../../../matrix-rank.md) and [trace](../../../../../../matrix-trace.md) $p$, and $I-H$ is the complementary [orthogonal projection](../../../../../../orthogonal-projection.md). Consequently

$$
\boxed{\operatorname{Cov}(\widehat Y)=\sigma^2HH^T=\sigma^2H,\qquad
\operatorname{Cov}(\widehat e)=\sigma^2(I-H).}
$$

Since $(I-H)X=0$, the [covariance matrix](../../../../../../covariance-matrix.md) between the [regression residual](../../../../../../regression-residual.md) vector and the coefficient estimate is

$$
\operatorname{Cov}(\widehat e,\widehat\beta)
=\sigma^2(I-H)X(X^TX)^{-1}=0.
$$

These quantities have a joint [normal distribution](../../../../../../normal-distribution.md), so they are also independent, a stronger conclusion than zero [covariance](../../../../../../covariance.md).

Now $\widehat e=(I-H)\varepsilon$ has mean zero. Using the expectation of a [quadratic form](../../../../../../quadratic-form.md),

$$
\mathbb E\,\mathrm{RSS}
=\mathbb E(\widehat e^T\widehat e)
=\operatorname{tr}\operatorname{Cov}(\widehat e)
=\sigma^2(n-p).
$$

Thus the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) has

$$
\mathbb E\widehat\sigma^2_{\mathrm{ML}}=\frac{n-p}{n}\sigma^2,
\qquad \operatorname{Bias}(\widehat\sigma^2_{\mathrm{ML}})=-\frac pn\sigma^2.
$$

The unbiased alternative is

$$
\boxed{s^2=\frac{\mathrm{RSS}}{n-p}.}
$$

The [orthogonal projection of a Gaussian vector](../../../../../../orthogonal-projection-of-a-gaussian-vector.md) also yields $\mathrm{RSS}/\sigma^2\sim\chi^2_{n-p}$, explaining the [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
