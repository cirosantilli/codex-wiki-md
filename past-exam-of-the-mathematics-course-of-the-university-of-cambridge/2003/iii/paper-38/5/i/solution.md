<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The independence analysis is not justified without further assumptions.** Three binary responses from the same subject generally remain correlated after conditioning on baseline [covariates](../../../../../../covariate.md) and treatment. The fitted independent-Bernoulli [likelihood](../../../../../../likelihood-function.md) discards that correlation and gives incorrect model-based [standard errors](../../../../../../standard-error.md) and tests if it is present. Positive within-subject correlation commonly makes those errors too small.

There is an important distinction between estimating the mean and estimating uncertainty. If the stated marginal [logistic regression](../../../../../../logistic-regression.md) is correct and responses are fully observed, the independence score $\sum_{i,j}w_{ij}(Y_{ij}-m_{ij})$ still has zero [expectation](../../../../../../expected-value.md). With independent subjects and regularity, its root can consistently estimate marginal coefficients despite within-subject dependence; a subject-level [sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md) is then needed. True independence is a special case in which the original [standard errors](../../../../../../standard-error.md) would be appropriate.

Dropout creates a separate issue. Restricting that score to observed responses need not preserve its zero [expectation](../../../../../../expected-value.md) if observation depends on the response history or unseen depression outcomes. Therefore both point estimates and uncertainty may be wrong. Neither random treatment assignment nor baseline adjustment alone establishes an [ignorable missingness mechanism](../../../../../../ignorable-missingness-mechanism.md). We need a model matched to the scientific estimand and explicit assumptions about [missing data](../../../../../../missing-data.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
