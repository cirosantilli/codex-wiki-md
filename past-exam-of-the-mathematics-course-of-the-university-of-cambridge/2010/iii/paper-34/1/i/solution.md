<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A reversal this large calls for an audit, but the aggregate table cannot identify a particular error. Check the outcome and exposure coding, the reference category, the subset used in each analysis, missing-data exclusions, denominators, weights, and whether the reported coefficient actually corresponds to the intended comparison. Reversing an exposure contrast or exponentiating the wrong fitted coefficient would change the reported [odds ratio](../../../../../../odds-ratio.md). Conditioning on variables affected by delivery, or including inappropriate interactions, could also change the [causal inference](../../../../../../causal-inference-split.md) rather than merely improve precision.

Start by reproducing the crude [odds ratio](../../../../../../odds-ratio.md) from an independent two-by-two calculation. Then fit progressively adjusted [logistic regressions](../../../../../../logistic-regression.md), recording how the coefficient and analysis population change; inspect within-clinic comparisons, sparse cells and [separation](../../../../../../separation-statistics.md). For an ordinary likelihood fit, check the fitted expected event count against the observed count and verify that changing only to cluster-robust standard errors leaves the fitted coefficients unchanged. A [sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md) corrects uncertainty for [clustered data](../../../../../../clustered-data.md); it does not by itself turn a crude odds ratio below one into an adjusted odds ratio above one. Adding clinic effects, using weights or changing the model can change the point estimate and must be distinguished from that variance correction.

**Programming or reporting error is a possibility to check, not a conclusion proved by the reversal**. Strong legitimate [confounding](../../../../../../confounding.md) remains another explanation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
