<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditional on the covariates, the binary responses are independent with [Bernoulli distributions](../../../../../../bernoulli-distribution.md):

$$
Y_i\sim\operatorname{Bernoulli}(p_i),\qquad\log\frac{p_i}{1-p_i}=\eta_i=\beta_0+\beta_I\,\mathrm{income}_i+\beta_A\,\mathrm{age}_i+\beta_L\,\mathrm{amount}_i.
$$

Thus $p_i=(1+e^{-\eta_i})^{-1}$, the [logistic regression](../../../../../../logistic-regression.md) model. The [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) are

$$
(\widehat\beta_0,\widehat\beta_I,\widehat\beta_A,\widehat\beta_L)=(-1.322701,-0.005916,-0.008580,0.012981).
$$

Using the reported age standard error, an approximate 95% [Wald confidence interval](../../../../../../wald-confidence-interval.md) is

$$
\boxed{-0.008580\pm1.96(0.003833)=[-0.01609268,-0.00106732]\approx[-0.01609,-0.00107].}
$$

This interval concerns the age coefficient in [log odds](../../../../../../log-odds.md) per year, with income and loan amount held fixed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
