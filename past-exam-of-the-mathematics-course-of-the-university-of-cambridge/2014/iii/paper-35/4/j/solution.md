<h1 id="4/j/solution">Solution</h1>

↑ **Parent:** [J](../j.md)

Fit both the normal and [Student t random-effect model](../../../../../../student-t-random-effect-model.md) with comparable proper [prior distributions](../../../../../../prior-probability.md). Compare priors on the same spread measure: a [normal distribution](../../../../../../normal-distribution.md) scale $\tau$ is a [standard deviation](../../../../../../standard-deviation.md), whereas the $t_4$ [standard deviation](../../../../../../standard-deviation.md) is $\sqrt2\psi$.

Use a [posterior predictive check](../../../../../../posterior-predictive-check.md): draw study effects and binomial counts from each fitted hierarchy and compare replicated dispersion and extreme study contrasts with the observations. For predicting a new study, generate a new effect from the hierarchy rather than reusing an existing fitted effect. A [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md) with entire studies held out can compare integrated predictive probabilities for both arms of each omitted trial, averaging over [hyperparameters](../../../../../../hyperparameter.md) and its unobserved study effect. [Leave-one-study-out influence analysis](../../../../../../leave-one-study-out-influence-analysis.md) also reveals whether the difference is driven by a single trial.

**Prefer the heavier-tailed hierarchy if it improves the relevant predictive checks and held-out study predictions robustly to reasonable prior choices.** The [deviance information criterion](../../../../../../deviance-information-criterion.md) can supplement the comparison, but its effective parameter count can depend on the latent-variable representation, and six studies give limited information about tail shape. A small numerical criterion difference alone is insufficient evidence.

## ↑ Ancestors (11)

1. [J](../j.md)
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
