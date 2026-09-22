<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The output must first identify the response scale and the formula. If the initial fit is ordinary least squares to the untransformed response with all fifteen predictors and an intercept, its [normal linear model](../../../../../../normal-linear-model.md) is

$$
Y=X\beta+\varepsilon,\qquad\varepsilon\sim N_{47}(0,\sigma^2I),\qquad\widehat\beta=(X^TX)^{-1}X^TY.
$$

For full rank $p=16$, the residual degrees of freedom are **$47-16=31$**. The [residual standard error](../../../../../../residual-standard-error.md) is $s=\sqrt{\operatorname{RSS}/31}$ and estimated coefficient covariance is $s^2(X^TX)^{-1}$. A coefficient test divides the estimate by its [standard error](../../../../../../standard-error.md) and compares with a $t_{31}$ reference distribution; the overall test of all fifteen slopes compares

$$
F=\frac{(\operatorname{RSS}_0-\operatorname{RSS})/15}{\operatorname{RSS}/31}
$$

with $F_{15,31}$. The intercept-only residual sum is $\operatorname{RSS}_0$. [Adjusted R-squared](../../../../../../adjusted-coefficient-of-determination.md) penalizes the loss of residual degrees of freedom, unlike ordinary $R^2$.

Each [regression coefficient](../../../../../../regression-coefficient.md) measures a conditional association holding the other columns fixed. The southern-state indicator compares two state categories at equal values of all other predictors. Rescaling changes the units of a coefficient, so one cannot infer effects per original currency unit or per original percentage unit without the scaling information. If the actual formula uses $\log y$, exponentiating a coefficient gives a multiplicative response change rather than an additive change; if both response and a predictor are logged, the slope is an elasticity. These interpretations cannot be interchanged.

The two police-expenditure variables are likely strongly associated and need a [multicollinearity](../../../../../../multicollinearity.md) check: individual coefficients can be unstable even when their joint contribution predicts well. Their actual correlation should be calculated, not presumed numerically. Similar considerations apply to age-specific unemployment. With only 47 observations and up to 16 mean parameters, examine [regression leverage](../../../../../../regression-leverage.md), [Cook's distance](../../../../../../cook-s-distance.md), residual distribution, variance versus fitted values, nonlinear effects and predictive [cross-validation](../../../../../../cross-validation.md). State-level geographical dependence may also violate the independent-error model.

The observations are aggregate states. An association between a state covariate and crime rate is not an individual causal effect: [ecological fallacy](../../../../../../ecological-fallacy.md), [confounding](../../../../../../confounding.md) and reverse causation are relevant. For example, greater recorded crime can induce greater police expenditure. **The absent coefficient table and model call prevent deciding which predictors were significant or even whether the fitted response was transformed.** The preceding degrees of freedom and formula interpretations are conditional on the explicitly stated full linear-model specification.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
