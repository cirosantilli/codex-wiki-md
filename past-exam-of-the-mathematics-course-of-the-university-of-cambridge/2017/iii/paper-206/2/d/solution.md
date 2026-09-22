<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [quasibinomial regression](../../../../../../quasibinomial-regression.md) retains the [logit link](../../../../../../logit.md) and mean function $p_i=(1+e^{-x_i^T\beta})^{-1}$ but uses the working [variance function](../../../../../../variance-function.md) $\operatorname{Var}(Y_i)=\phi p_i(1-p_i)$. Its [quasi-score equation](../../../../../../quasi-score-equation.md) is

$$
U(\beta)=\phi^{-1}\sum_i x_i(y_i-p_i)=0,
$$

so multiplying by the common [dispersion parameter](../../../../../../dispersion-parameter.md) does not change the coefficient estimates. [Iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md) therefore gives the same fitted means and coefficients as the binomial model. The usual [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md) is

$$
\widehat\phi=\frac{1}{120-2}\sum_i\frac{(y_i-\widehat p_i)^2}{\widehat p_i(1-\widehat p_i)}.
$$

The estimated coefficient [covariance matrix](../../../../../../covariance-matrix.md) is $\widehat\phi(X^TWX)^{-1}$, with $W_{ii}=\widehat p_i(1-\widehat p_i)$. From the intercept [standard errors](../../../../../../standard-error.md), $(1.08921/1.13031)^2\simeq0.92860$; the rounded slope errors give approximately the same factor. The display uses approximate [Student's t-tests](../../../../../../student-s-t-test.md) with 118 [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md) instead of fixed-dispersion normal tests.

For a genuinely individual binary response, the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) identity $Y_i^2=Y_i$ forces $\operatorname{Var}(Y_i)=p_i(1-p_i)$. Thus $\phi\ne1$ is a working [quasi-likelihood](../../../../../../quasi-likelihood.md) specification, not a different independent binary distribution with that mean. The mild estimated [underdispersion](../../../../../../underdispersion.md) does not establish an improved model, and the mean predictions are unchanged. In particular, a scalar rescaling does not model correlation among users, and usual likelihood-based [Akaike information criterion](../../../../../../akaike-information-criterion.md) comparisons are unavailable for a family without a specified probability likelihood. **The output gives no convincing reason to prefer model3 to model2.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
