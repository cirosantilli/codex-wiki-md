<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

The first command fits independent [Poisson random variables](../../../../../poisson-distribution.md) with means $\mu_j$ and a [log link](../../../../../logarithmic-link-function.md). For concentration $x$ and strain indicator $s$, its fitted [linear predictor](../../../../../linear-predictor.md) is

$$
\log\widehat\mu=4.14443-1.47253x+0.33667s-0.12534xs.
$$

The [interaction](../../../../../interaction-statistics.md) allows different concentration slopes in the two strains. At $x=0$ the second strain's mean is multiplied by $e^{0.33667}$; its slope is $-1.47253-0.12534$. These are multiplicative changes in counts, not changes in probabilities.

The [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) use the [Poisson regression](../../../../../poisson-regression.md) likelihood. With [design matrix](../../../../../design-matrix.md) $X$, estimated information $X^T\operatorname{diag}(\widehat\mu_j)X$ gives the inverse [covariance matrix](../../../../../covariance-matrix.md); diagonal square roots give the [standard errors](../../../../../standard-error.md). The printed [Wald tests](../../../../../wald-test.md) use approximately standard-normal coefficient-to-error ratios. Fuel and strain effects are strong, whereas the [interaction](../../../../../interaction-statistics.md) has $p=0.182$, suggesting a common slope.

$H_2$ removes just the [interaction](../../../../../interaction-statistics.md); $H_3$ also removes strain. Their parameter counts are four, three and two. Under the usual large-sample [likelihood-ratio test](../../../../../likelihood-ratio-test.md), $D_2-D_1=1.78089$ is compared with $\chi^2_1$ and is below $3.841459$, so the [interaction](../../../../../interaction-statistics.md) is not required at 5%. By contrast, $D_3-D_2=32.61857$ is far above that threshold, so the strain main effect should remain. Comparing $H_3$ directly with $H_1$ uses $D_3-D_1$ and two [degrees of freedom](../../../../../degree-of-freedom.md).

For an approximate absolute goodness-of-fit test, compare $D_1=84.59557$ with $\chi^2_{70-4}$; its upper-tail probability is about $0.061$. For $H_2$, $D_2=86.37646$ on $67$ [degrees of freedom](../../../../../degree-of-freedom.md) has $p\approx0.056$. **The additive model $H_2$ is the preferred parsimonious fit** at 5%, subject to the independent [Poisson distribution](../../../../../poisson-distribution.md) and large-sample assumptions. The printed nine rows are only a subset; the supplied fitted output refers to all 70 observations.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
