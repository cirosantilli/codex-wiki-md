# Conditional multinomial sufficient statistics

↑ **Parent:** [Multinomial logistic regression](multinomial-logistic-regression.md)

For independent [multinomial distributions](multinomial-distribution.md) with fixed stratum totals $N_s$ and baseline logits $\log(p_{sl}/p_{sL})=x_s^T\beta_l$, the [sufficient statistics](sufficient-statistic.md) are the displayed response-specific design-weighted counts, $l<L$. Expanding the [log-likelihood](log-likelihood.md) gives $\sum_{l<L}\beta_l^TT_l-\sum_sN_s\log(1+\sum_{l<L}e^{x_s^T\beta_l})$, plus a data-only term. The [Fisher-Neyman factorization theorem](fisher-neyman-factorization-theorem.md) therefore proves sufficiency; with an unrestricted identifiable canonical parameter, a likelihood-ratio argument proves minimal sufficiency. Factor indicators give the corresponding response/covariate margins.

## ↑ Ancestors (9)

1. [Multinomial logistic regression](multinomial-logistic-regression.md)
2. [Logistic regression](logistic-regression.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
