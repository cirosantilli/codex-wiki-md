<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [independent](../../../../../../independent-random-variables.md) standard [Cauchy distribution](../../../../../../cauchy-distribution.md) draws $X_1,\ldots,X_n$, the code averages the indicators $I_i=\mathbf1_{\{X_i>2\}}$. Each is a [Bernoulli random variable](../../../../../../bernoulli-distribution.md) with parameter

$$
\theta=\int_2^\infty\frac{dx}{\pi(1+x^2)}=\frac12-\frac{\arctan2}{\pi}=\frac{\arctan(1/2)}\pi.
$$

Hence it is an [unbiased estimator](../../../../../../unbiased-estimator.md) of that tail probability, and [independence](../../../../../../independent-random-variables.md) gives

$$
\boxed{\widehat\theta=\frac1n\sum_{i=1}^n I_i,\qquad\theta\approx0.1475836,\qquad\operatorname{Var}(\widehat\theta)=\frac{\theta(1-\theta)}n.}
$$

The [variance](../../../../../../variance-split.md) is finite even though the underlying Cauchy draws have no finite mean: the variables being averaged are bounded indicators, not the Cauchy values themselves.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
