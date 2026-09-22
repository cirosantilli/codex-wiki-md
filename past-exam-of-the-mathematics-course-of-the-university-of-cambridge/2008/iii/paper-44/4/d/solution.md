<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Model B replaces independent tree parameters by [multivariate normal](../../../../../../multivariate-normal-distribution.md) [random effects](../../../../../../random-effect.md). It permits correlated asymptote, timing and slope variation and supplies [partial pooling](../../../../../../partial-pooling.md), a useful improvement if the five trees can be regarded as [exchangeable](../../../../../../exchangeable-random-variables.md).

The [Wishart distribution](../../../../../../wishart-distribution.md) prior is on the [precision matrix](../../../../../../precision-matrix.md) $\Omega$, not the covariance matrix. In the [WinBUGS](../../../../../../winbugs.md) convention, dimension three and degrees of freedom three give a proper but very dispersed prior. The induced [inverse-Wishart distribution](../../../../../../inverse-wishart-distribution.md) has no finite mean at those degrees of freedom. Thus this is not a neutral choice of covariance prior, and estimating six covariance components from only five trees is weakly informed. The broad mean priors and possible negative growth slopes also remain. Check prior-predictive curves and sensitivity, and consider separate, interpretable scale and correlation priors.

The resulting posterior means of the second and third parameters are quite similar across trees, motivating a simpler shared-shape model; their uncertainty means this similarity is evidence to explore, rather than a proof of exact equality.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
