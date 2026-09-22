<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a baseline-adjusted [linear regression](../../../../../../linear-regression-split.md) for an [intention-to-treat analysis](../../../../../../intention-to-treat-analysis.md):

$$
Y_i=\alpha+\beta Z_i+\gamma^{\mathsf T}x_i+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{ind}}\sim N(0,\sigma^2).
$$

Condition on the observed [baseline covariates](../../../../../../baseline-covariate.md) and assignment. The parameter of primary interest is **$\beta$, the mean effect of assignment to the experimental intervention**, under this constant-effect conditional mean model. Independent [normal distributions](../../../../../../normal-distribution.md) with common [variance](../../../../../../variance-split.md) give the usual Gaussian [likelihood](../../../../../../likelihood-function.md) and regression inference. Prognostic [baseline covariates](../../../../../../baseline-covariate.md) improve precision by explaining outcome variability.

Do not include the actual intervention-use variable $D_i$ as an ordinary adjustment variable for this estimand: it is measured after assignment and can mediate the effect being estimated. [Post-randomization adjustment changes a treatment estimand](../../../../../../post-randomization-adjustment-changes-a-treatment-estimand.md); the resulting coefficient on $Z_i$ would generally represent a different comparison. Participants remain in their assigned groups even when adherence differs.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
