<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The derivation extends to either actual model once its formula is known. If $x_{ijk}$ is its covariate design vector and the baseline logits are $x_{ijk}^T\beta_l$, then

$$
\ell(\beta)=\sum_{l<L}\beta_l^T\underbrace{\sum_{ijk}n_{ijkl}x_{ijk}}_{T_l}-\sum_{ijk}N_{ijk}\log\left(1+\sum_{l<L}e^{x_{ijk}^T\beta_l}\right)+\log h(n).
$$

Thus **the conditional multinomial sufficient statistics are $T_l=\sum_{ijk}n_{ijkl}x_{ijk}$, for $l<L$**. For an identifiable unrestricted canonical parameter space they are also minimal up to linear equivalence: the ratio of two data likelihoods is parameter-independent exactly when the differences of all these design-weighted sums vanish. This follows because that ratio contains $\exp\{\sum_l\beta_l^T(T_l(n)-T_l(n'))\}$.

Consequently an influence-by-type response interaction adds the margins $n_{ij+l}$; influence-by-contact adds $n_{i+kl}$; type-by-contact adds $n_{+jkl}$. A saturated model requires the individual cells, subject to the fixed stratum totals. A hierarchical [log-linear model](../../../../../../log-linear-model.md) leads to the same response/covariate margins and the fixed covariate margin. There is no need to guess sufficient statistics from the number of displayed coefficients: they follow from the actual design columns and the likelihood.

To read a printed fit, check whether it is a Poisson surrogate, a baseline-category multinomial model or an ordinal cumulative model, then inspect its reference levels, signs of response contrasts, [standard errors](../../../../../../standard-error.md), residual [deviance](../../../../../../exponential-family-deviance.md), degrees of freedom, nested comparisons and predicted probabilities. A baseline-logit coefficient changes odds of one satisfaction level against the baseline, not necessarily cumulative odds of high satisfaction. Normalize Poisson fitted counts within each covariate stratum to get fitted response probabilities. Empty or sparse cells can cause boundary fits or invalidate a naive deviance reference distribution.

A [proportional-odds model](../../../../../../proportional-odds-model.md) instead specifies $\operatorname{logit}P(Y\le l\mid x)=\theta_l-x^T\beta$. It uses the response ordering, with shared slopes across cutpoints. Its category probabilities are differences of cumulative logistic probabilities, so its log-likelihood is not the canonical linear expression above. The baseline-category margins just derived are not generally sufficient for that model; the full conditional cell table is always sufficient. **Without the missing formulas it is not possible to certify which two specific models were fitted or their actual sufficient-margin lists and test results.** The null, additive and general-design derivations above state precisely which model each answer belongs to.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
