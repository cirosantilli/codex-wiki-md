<h1 id="13j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fit a [Poisson regression](../../../../../../poisson-regression.md) to artificial responses $Z_i=1$ with means

$$
\mu_i=\Lambda(Y_i)e^{\beta^Tx_i}.
$$

With the logarithmic link, this is the [generalized linear model](../../../../../../generalized-linear-model.md)

$$
\log\mu_i=\beta^Tx_i+\log\Lambda(Y_i),
$$

where $\log\Lambda(Y_i)$ is a known offset. Its log likelihood, apart from constants, is

$$
\ell_P(\beta)
=\sum_i[\log\Lambda(Y_i)+\beta^Tx_i-\Lambda(Y_i)e^{\beta^Tx_i}].
$$

The difference

$$
\ell(\beta)-\ell_P(\beta)
=\sum_i[\log\lambda(Y_i)-\log\Lambda(Y_i)]
$$

does not depend on $\beta$. **The Poisson surrogate therefore has exactly the same maximum-likelihood estimate of $\beta$.** This is the [Poisson surrogate for an uncensored proportional-hazards likelihood](../../../../../../poisson-surrogate-for-an-uncensored-proportional-hazards-likelihood.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
