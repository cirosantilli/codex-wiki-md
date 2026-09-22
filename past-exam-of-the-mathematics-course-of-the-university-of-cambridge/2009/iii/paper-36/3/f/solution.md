<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Under the common observation-level [Bayesian deviance](../../../../../../bayesian-deviance.md) convention, [DIC](../../../../../../deviance-information-criterion.md) is $\overline D+p_D$, with the [effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md) defined by $p_D=\overline D-D(\overline\psi)$. The no-random-effect model's effective count is near three, corresponding to its three fitted regression coefficients. With plate [random effects](../../../../../../random-effect.md), the effective count rises to $13.6$: the local effects add flexibility, but their partial pooling means they do not count as eighteen fully independent unrestricted fitted parameters. The effective count need not be an integer or equal the raw parameter count; the scale parameter controls that shrinkage.

Adding the plate effects reduces the average [Bayesian deviance](../../../../../../bayesian-deviance.md) by $28.6$ at an effective-complexity cost of $10.7$. Therefore its [DIC](../../../../../../deviance-information-criterion.md) is lower by

$$
\boxed{142.1-124.2=17.9.}
$$

**The reported criterion favours the overdispersed model.** This is a fit-complexity comparison, not a posterior probability or [Bayes factor](../../../../../../bayes-factor.md). In a [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md), the interpretation depends on whether deviance is conditional on local effects or has marginalized them out; these figures use the supplied observation-level convention.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
