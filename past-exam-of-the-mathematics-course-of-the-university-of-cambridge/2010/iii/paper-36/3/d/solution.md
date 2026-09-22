<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\overline\theta=\mathbb E(\theta\mid y)$ and $\overline D=\mathbb E\{D(\theta)\mid y\}$. The usual [effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md) is

$$
\boxed{p_D=\overline D-D(\overline\theta).}
$$

With the locally flat [prior distribution](../../../../../../prior-probability.md), $\overline\theta\approx\widehat\theta$ and the mean of the [chi-squared distribution](../../../../../../chi-squared-distribution.md) excess is $p$. Thus $\overline D\approx D(\widehat\theta)+p$, while $D(\overline\theta)\approx D(\widehat\theta)$, giving **$p_D\approx p$**.

More generally, the [quadratic posterior deviance moments](../../../../../../quadratic-posterior-deviance-moments.md) give the effective count. Within the same approximation, let the [posterior covariance matrix](../../../../../../posterior-covariance-matrix.md) be $\Sigma$. The expectation of a [quadratic form](../../../../../../quadratic-form.md) gives

$$
\overline D\approx D(\widehat\theta)+(\overline\theta-\widehat\theta)^TJ(\overline\theta-\widehat\theta)+\operatorname{tr}(J\Sigma),
$$

whereas evaluation at $\overline\theta$ omits the trace term. Therefore $p_D\approx\operatorname{tr}(J\Sigma)$. For a flat prior, $\Sigma\approx J^{-1}$ and the trace is $p$; informative prior shrinkage can reduce this effective count.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
