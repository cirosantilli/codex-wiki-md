<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The printed formula expands to the main effects of school type, acceptance and college, together with school-type-by-college and acceptance-by-college interactions. It contains neither a school-type-by-acceptance interaction nor the corresponding three-way interaction. Its [Poisson regression](../../../../../../poisson-regression.md) model is therefore

$$
\log\mu_{abj}=\gamma_j+\alpha_{aj}+\beta_{bj}.
$$

For every college the mean table has [odds ratio](../../../../../../odds-ratio.md)

$$
\boxed{\frac{\mu_{11j}\mu_{22j}}{\mu_{12j}\mu_{21j}}=1.}
$$

Thus it tests [conditional independence](../../../../../../conditional-independence.md) of school type and acceptance given college, while permitting both margins to vary freely across colleges. It does not merely assert a common, possibly nonzero association.

The [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) score equations match every school-type-by-college and acceptance-by-college margin. Solving them gives the [stratified two-by-two conditional independence model](../../../../../../stratified-two-by-two-conditional-independence-model.md)'s fitted counts

$$
\boxed{\widehat\mu_{abj}=\frac{n_{a+j}n_{+bj}}{n_{++j}}.}
$$

Indeed these counts factor by row and column and have exactly the observed margins. For nondegenerate tables there are three free mean parameters per college: one total and two independent margin proportions. There are $100$ cells and $75$ parameters, hence **25 residual degrees of freedom**. The residual [deviance](../../../../../../exponential-family-deviance.md) is

$$
G^2=2\sum_{a,b,j}n_{abj}\log\frac{n_{abj}}{\widehat\mu_{abj}},
$$

with zero-count contributions interpreted as zero. The Poisson linear terms cancel because the fitted totals equal the observed totals. Under the null and suitable large-count regularity, compare $G^2$ with $\chi^2_{25}$. Sparse cells, structural zeros or degenerate margins require a different calibration, such as an appropriate conditional test or simulated reference distribution.

A large residual [deviance](../../../../../../exponential-family-deviance.md) is evidence of school-type/acceptance association in at least some colleges. A small one indicates compatibility with conditional independence, not proof of identical admission processes or absence of selection on qualifications. Residuals and individual college contrasts locate departures. Adding the school-type-by-acceptance term gives a common [odds ratio](../../../../../../odds-ratio.md), one extra parameter and 24 residual degrees of freedom. Adding the full three-way term permits each college's association and saturates the tables. The first comparison tests a common association; the second checks whether a common association is adequate. No frequencies are supplied here to evaluate these tests numerically.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
