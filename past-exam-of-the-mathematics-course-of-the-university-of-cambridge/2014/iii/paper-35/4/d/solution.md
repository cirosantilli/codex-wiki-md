<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Calling the effects [exchangeable random variables](../../../../../../exchangeable-random-variables.md) means that their joint [prior distribution](../../../../../../prior-probability.md) is unchanged by permuting study labels. In a [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md), conditional independent draws $\beta_j\mid\mu,\tau\sim N(\mu,\tau^2)$ achieve this, and integrating shared [hyperparameters](../../../../../../hyperparameter.md) induces dependence between studies. This permits [partial pooling](../../../../../../partial-pooling.md) without asserting that all effects are identical.

The assumption is reasonable when the studies concern comparable treatments, populations, outcomes and follow-up, and no known study characteristic gives one effect a systematically different prior center. Relevant differences can instead enter a [linear regression](../../../../../../linear-regression-split.md) for study effects, after which the residual effects may be exchangeable. **The numerical table counts deaths**, so its event probabilities are mortality probabilities and $\beta_j<0$ indicates a lower mortality [odds ratio](../../../../../../odds-ratio.md). Interpreting those counts as beneficial responses would reverse the clinical meaning.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
