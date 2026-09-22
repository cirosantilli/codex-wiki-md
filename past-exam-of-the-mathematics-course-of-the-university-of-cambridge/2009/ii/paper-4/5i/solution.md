<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The fit is a [Gaussian linear model](../../../../../normal-linear-model.md) for $Y_i=\log(\mathrm{so2}_i)$ with an intercept and the six displayed explanatory variables:

$$
Y_i=\beta_0+\beta_1\mathrm{temp}_i+\beta_2\mathrm{manuf}_i+\beta_3\mathrm{pop}_i+\beta_4\mathrm{wind}_i+\beta_5\mathrm{precip}_i+\beta_6\mathrm{days}_i+\varepsilon_i,
\qquad \varepsilon_i\overset{\rm iid}{\sim}N(0,\sigma^2).
$$

The command computes [ordinary least squares](../../../../../ordinary-least-squares.md); independent normal errors with common [variance](../../../../../variance-split.md) are the additional assumptions yielding the exact printed tests. A coefficient describes an adjusted association on the log scale, holding the other variables fixed. Exponentiation gives a multiplicative effect on the conditional median of sulphur dioxide, not an additive effect on its original scale. Under the Gaussian model its conditional mean additionally includes the factor $e^{\sigma^2/2}$.

The estimates are the coordinates of $\widehat\beta=(X^TX)^{-1}X^TY$. With $41$ observations and $7$ parameters the residual degrees of freedom are $34$, and the [residual standard error](../../../../../residual-standard-error.md) is $s=\sqrt{\mathrm{RSS}/34}=0.448$ to the displayed precision. The reported [standard error](../../../../../standard-error.md) of coefficient $j$ is $s\sqrt{[(X^TX)^{-1}]_{jj}}$. For each [null hypothesis](../../../../../null-hypothesis.md) $\beta_j=0$, the displayed statistic $t_j=\widehat\beta_j/\operatorname{se}(\widehat\beta_j)$ has [Student t-distribution](../../../../../student-s-t-distribution.md) with $34$ degrees of freedom under that null. Its two-sided [p-value](../../../../../p-value.md) is $2\Pr(t_{34}\ge|t_j|)$.

At the $5\%$ level the intercept, temperature, manufacturing and wind coefficients differ significantly from zero in the full model. Temperature and wind have negative estimated adjusted effects; manufacturing has a positive one. The p-values for population, precipitation and precipitation days, approximately $0.136$, $0.127$ and $0.931$, do not reject their respective zero-coefficient hypotheses. This is not evidence that their effects are exactly zero, and these observational associations do not establish causation.

A sensible candidate reduced [linear regression](../../../../../linear-regression-split.md) keeps an intercept, temperature, manufacturing and wind. It must be refitted: coefficients generally change when correlated predictors are removed. The three deletions can be checked jointly by the [F-test](../../../../../f-test.md) statistic

$$
F=\frac{(\mathrm{RSS}_{\rm reduced}-\mathrm{RSS}_{\rm full})/3}{\mathrm{RSS}_{\rm full}/34},
$$

which has $F_{3,34}$ distribution under the joint null. The individual summary does not determine this joint test or establish the reduced model's adequacy.

In the final command, the uniquely matching component named by `fit$df` is the residual degrees of freedom. Thus the result is $\boxed{\sqrt{\mathrm{RSS}/34}=0.448\text{ to printed precision}.}$

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
