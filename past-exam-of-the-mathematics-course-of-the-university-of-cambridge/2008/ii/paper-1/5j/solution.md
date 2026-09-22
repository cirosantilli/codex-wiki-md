<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

The inverse [logit link](../../../../../logit.md) is $\mu_i(\beta)=e^{\beta^Tx_i}/(1+e^{\beta^Tx_i})$. [independence](../../../../../independent-random-variables.md) therefore gives the [Likelihood function](../../../../../likelihood-function.md) and [log-likelihood](../../../../../log-likelihood.md)

$$
\boxed{L(\beta;y)=\prod_i\mu_i^{y_i}(1-\mu_i)^{1-y_i},\qquad
\ell(\beta)=\sum_i\left[y_i\beta^Tx_i-\log(1+e^{\beta^Tx_i})\right].}
$$

Differentiation yields the score $\nabla_\beta\ell=\sum_i x_i(y_i-\mu_i)$. The matrix whose rows are $x_i^T$ has dimension $n\times p$, not the PDF's printed $p\times n$. With this necessary dimension correction, any finite maximum [Likelihood function](../../../../../likelihood-function.md) estimate satisfies

$$
\boxed{X^Ty=X^T\widehat\mu,\qquad
\widehat\mu_i=\frac{e^{\widehat\beta^Tx_i}}{1+e^{\widehat\beta^Tx_i}}.}
$$

The [Hessian matrix](../../../../../hessian-matrix.md) is $-X^TWX$, with $W_{ii}=\mu_i(1-\mu_i)$, so the [log-likelihood](../../../../../log-likelihood.md) is concave. These score equations apply to a finite interior estimate; complete or quasi-complete separation can instead make its supremum occur only as coefficients diverge.

The [deviance](../../../../../exponential-family-deviance.md) is twice the difference between maximized saturated and fitted [log-likelihoods](../../../../../log-likelihood.md). A saturated [Bernoulli distribution](../../../../../bernoulli-distribution.md) has fitted means $y_i\in\{0,1\}$ and [log-likelihood](../../../../../log-likelihood.md) zero, interpreted by limits. Hence the [binomial deviance](../../../../../binomial-deviance.md) here is

$$
\boxed{D(y;\widehat\mu)=2\sum_i\left[y_i\log\frac{y_i}{\widehat\mu_i}+(1-y_i)\log\frac{1-y_i}{1-\widehat\mu_i}\right]
=-2\sum_i\left[y_i\log\widehat\mu_i+(1-y_i)\log(1-\widehat\mu_i)\right].}
$$

Zero-multiplier logarithms are interpreted as zero.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
