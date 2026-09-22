<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md) separates variability between individuals from variability between repeated measurements on an individual. In [WinBUGS](../../../../../../winbugs.md), `dnorm` takes a [precision parameter](../../../../../../precision-parameter.md), so inverse variance is the appropriate second argument.

Line (1) gives $\log\sigma_j^2\sim N(\phi,\psi^2)$, hence a positive [log-normal distribution](../../../../../../log-normal-distribution.md) for each within-individual variance. Estimating the shared parameters supplies [partial pooling](../../../../../../partial-pooling.md) of these variances without forcing them equal. Line (2) assigns a proper bounded flat prior to the between-individual standard deviation $\tau$, and line (3) does the same for the standard deviation $\psi$ on the log-variance scale. The broad bounded priors on $\mu$ and $\phi$ are also proper.

This is a reasonable structure for heterogeneous repeated measurements, but flat does not mean uninformative on all transformed scales. The bounds must be wide enough for plausible values, while such enormous ranges can put substantial mass on implausible predictions. Use [prior predictive checks](../../../../../../prior-predictive-check.md) and sensitivity analysis, and check the [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md). Serial dependence or systematic trends would require an extension of the independent-measurement likelihood.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
