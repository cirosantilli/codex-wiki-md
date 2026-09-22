<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Write $Y_i=\log(\mathrm{price}_i)$ and fit the [normal linear model](../../../../../normal-linear-model.md)

$$
Y_i=\beta_0+\beta_1\mathrm{mpg}_i+\beta_2\mathrm{psngr}_i+
\beta_3\mathrm{length}_i+\beta_4\mathrm{width}_i+
\beta_5\mathrm{weight}_i+\varepsilon_i.
$$

The basic [linear regression](../../../../../linear-regression-split.md) analysis assumes centered independent [normal random variables](../../../../../gaussian-random-variable.md) $\varepsilon_i$ of a common [variance](../../../../../variance-split.md) $\sigma^2$, conditional on the predictors. Independence between makes does not by itself establish independence between different models of the same make; that stronger assumption should be checked, or within-make dependence modelled. The requested R fit is

```
fit <- lm(log(price) ~ mpg + psngr + length + width + weight, data = cars)
```

The estimate column contains the [ordinary least squares](../../../../../ordinary-least-squares.md) coefficients. The standard error estimates the [standard deviation](../../../../../standard-deviation.md) of each coefficient estimator. The t value is its estimate divided by its standard error. The last column gives the two-sided [p-value](../../../../../p-value.md) for a zero coefficient, using a [Student t-distribution](../../../../../student-s-t-distribution.md) with $93-6=87$ residual degrees of freedom under the stated [normal linear model](../../../../../normal-linear-model.md); the stars summarize significance thresholds.

Conditional on the other predictors, passenger capacity and width have negative fitted coefficients, while length and weight have positive ones. All four are significant at the conventional 5% level; length is borderline. There is little evidence for an additional mpg effect once the others are included. These are conditional associations, not causal claims. For example, increasing weight by 100 pounds multiplies the fitted price by approximately $\exp(0.08373)$, about 1.087.

A reasonable candidate simplification removes mpg and compares the nested models by an [F-test](../../../../../f-test.md), rather than treating a nonsignificant coefficient as proof of no effect:

```
fit2 <- update(fit, . ~ . - mpg)
anova(fit2, fit)
```

Inspect [regression residuals](../../../../../regression-residual.md), normal quantiles, residual-versus-fitted plots, leverage and influential observations. The correlated size predictors may produce [multicollinearity](../../../../../multicollinearity.md); missing make effects, nonlinear terms or unequal residual variances may also matter. A random make effect or a covariance adjustment addresses the possible dependence noted above.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
