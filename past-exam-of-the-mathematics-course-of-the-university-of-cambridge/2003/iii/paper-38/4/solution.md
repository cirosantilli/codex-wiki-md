<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use $\alpha$ for the intercept, to avoid confusing it with the observation means. Let $e_i=\exp(\widehat\alpha+\widehat\beta^Tx_i)$ be the fitted [Poisson regression](../../../../../poisson-regression.md) mean. Apart from constants, its [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(\alpha,\beta)=\sum_i\{y_i(\alpha+\beta^Tx_i)-\exp(\alpha+\beta^Tx_i)-\log(y_i!)\}.
$$

At a finite interior [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md), the intercept [score equation](../../../../../score-equation.md) gives the [Poisson regression margin-matching score equations](../../../../../poisson-regression-margin-matching-score-equations.md):

$$
\frac{\partial\ell}{\partial\alpha}=\sum_i(y_i-e_i)=0,\qquad\boxed{\sum_i e_i=\sum_i y_i.}
$$

The [statistical saturated model](../../../../../saturated-statistical-model.md) fits each mean to $y_i$, taking the boundary mean zero if $y_i=0$. Subtracting fitted from saturated [log-likelihood](../../../../../log-likelihood.md) gives the [Poisson deviance](../../../../../poisson-deviance.md)

$$
D=2\sum_i\left[y_i\log\frac{y_i}{e_i}-(y_i-e_i)\right].
$$

The intercept balance cancels the sum of linear terms. Consequently

$$
\boxed{D=2\sum_i y_i\log(y_i/e_i),\qquad0\log(0/e_i)=0.}
$$

The unsimplified formula makes nonnegativity transparent; individual terms in the simplified formula need not each be positive.

For the [deviance goodness-of-fit test](../../../../../deviance-goodness-of-fit-test.md), if the fitted design has rank $r$, compare a suitably calibrated $D$ with $\chi^2_{n-r}$, rejecting for large values. This approximation applies in a regular large-count regime, such as a fixed set of cells with increasing exposure and positive fitted proportions. It is not automatically accurate for many sparse [Poisson](../../../../../poisson-distribution.md) observations. Check residual patterns and [overdispersion](../../../../../overdispersion.md); where the approximation is doubtful, simulate independent [Poisson random variables](../../../../../poisson-distribution.md) with fitted means, refit each sample, and use a [parametric bootstrap](../../../../../parametric-bootstrap.md) distribution of the same statistic. A large [p-value](../../../../../p-value.md) means no detected lack of fit, not proof of the model. If a finite interior estimate fails to exist, the score proof needs a boundary-limit interpretation; for example all-zero data give a supremum with every fitted mean tending to zero and limiting deviance zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
