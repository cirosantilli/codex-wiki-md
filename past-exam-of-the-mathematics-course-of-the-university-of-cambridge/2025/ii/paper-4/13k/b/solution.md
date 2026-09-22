<h1 id="13k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The estimates maximize the grouped-binomial likelihood, numerically obtained by [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). At the fitted probabilities, the estimated covariance matrix is the inverse observed information, approximately

$$
\widehat{\operatorname{Var}}(\widehat\beta)
=(X^T\widehat W X)^{-1},
\qquad
\widehat W_{ii}=n_i\widehat p_i(1-\widehat p_i).
$$

The `Std. Error` column is the square root of its diagonal. Each `z value` is `Estimate/Std. Error`, and the two-sided [Wald test](../../../../../../wald-test.md) p-value is

$$
2\Phi(-|z|)
$$

for the null hypothesis that the corresponding coefficient is zero.

Thus $\widehat\beta_0=1.6855$ is the fitted log odds for a nonmalignant patient at site A. The site coefficients compare B and C with A, while $\widehat\beta_M=-0.9048$ compares malignant with nonmalignant tumours after adjustment for site. In odds-ratio form,

$$
e^{0.8096}\approx2.25,
\qquad e^{-0.5423}\approx0.58,
\qquad e^{-0.9048}\approx0.405.
$$

At level $0.05$, the B-versus-A contrast is not significant ($p=0.0624$), the C-versus-A contrast is not significant ($p=0.2610$), and malignancy has a significant negative association with survival ($p=0.0175$). The intercept test merely compares the baseline survival probability with $1/2$.

The null deviance $11.693$ compares the intercept-only fit with the saturated model and has $6-1=5$ residual degrees of freedom. The residual deviance $0.85048$ compares the four-parameter fitted model with the saturated model and has $6-4=2$ degrees of freedom. Finally, the [Akaike information criterion](../../../../../../akaike-information-criterion.md) is

$$
\boxed{-2\ell(\widehat\beta)+2\cdot4=29.003.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13K](../../13k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
