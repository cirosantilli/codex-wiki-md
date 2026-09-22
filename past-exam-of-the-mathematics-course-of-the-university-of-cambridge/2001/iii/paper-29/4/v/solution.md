<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use a [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md) with binomial observation errors and a common distribution for the underlying risks:

$$
D_j\mid p_j,n_j\sim\operatorname{Binomial}(n_j,p_j),\qquad
p_j\mid\alpha,\beta\ \overset{\mathrm{ind}}\sim\operatorname{Beta}(\alpha,\beta),\qquad j=1,\ldots,n.
$$

Give $(\alpha,\beta)$ a shared hyperprior, or parameterize them by mean $m=\alpha/(\alpha+\beta)$ and concentration $\kappa=\alpha+\beta$ and put priors on $m\in(0,1)$ and $\kappa>0$. Conditional on these hyperparameters, the risks are independent and identically distributed; after integrating them out they are [exchangeable random variables](../../../../../../exchangeable-random-variables.md) with shared uncertainty. The data estimate the overall risk level and between-hospital variation. Conditional [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md) gives

$$
p_j\mid\alpha,\beta,D_j\sim\operatorname{Beta}(\alpha+D_j,\beta+n_j-D_j),
$$

and full Bayes point estimates under [squared-error loss](../../../../../../squared-error-loss.md) are

$$
\boxed{\mathbb E[p_j\mid\boldsymbol D]=\mathbb E\left[\frac{\alpha+D_j}{\alpha+\beta+n_j}\,\middle|\,\boldsymbol D\right].}
$$

An [Empirical Bayes method](../../../../../../empirical-bayes-method.md) instead estimates the hyperparameters from the marginal [beta-binomial distribution](../../../../../../beta-binomial-distribution.md) [likelihood](../../../../../../likelihood-function.md)

$$
\prod_j\binom{n_j}{D_j}\frac{B(\alpha+D_j,\beta+n_j-D_j)}{B(\alpha,\beta)}
$$

and inserts their fitted values in the conditional posterior means. Both approaches provide partial pooling, stronger for smaller hospitals. Full Bayes also propagates hyperparameter uncertainty into the [credible intervals](../../../../../../credible-interval.md). If systematic [covariates](../../../../../../covariate.md) are needed, one can place exchangeable residual effects in a [logistic regression](../../../../../../logistic-regression.md) model rather than assuming a common unconditional risk distribution.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
