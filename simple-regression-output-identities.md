# Simple-regression output identities

↑ **Parent:** [Simple linear regression](simple-linear-regression.md)

Consider [ordinary least squares](ordinary-least-squares.md) with an [intercept](regression-intercept.md), one nonconstant predictor, $n>2$ cases, $S_{xx}=\sum_i(x_i-\bar x)^2>0$ a nonconstant response, and a positive [residual sum of squares](residual-sum-of-squares.md). With the usual common-variance [standard error](standard-error.md), put $s^2=\operatorname{RSS}/(n-2)$. Then

$$
\bar y=\widehat\alpha+\widehat\beta\bar x,\qquad \operatorname{SE}(\widehat\beta)=s/\sqrt{S_{xx}},\qquad F=t_{\mathrm{slope}}^2=\frac{(n-2)R^2}{1-R^2}.
$$

The [least-squares normal equations](normal-equations-for-linear-least-squares.md) give zero residual sum and zero residual [inner product](inner-product-split.md) with the centred predictor, proving the first identity and $\widehat\beta=S_{xy}/S_{xx}$. The fitted centred [sum of squares](sum-of-squares.md) is $\widehat\beta^2S_{xx}$. Dividing it by $s^2$ gives the one-predictor F statistic and the squared zero-slope t statistic. Dividing fitted and [residual sums of squares](residual-sum-of-squares.md) by their total gives the last expression. If $0\le R^2<1$, the [adjusted coefficient of determination](adjusted-coefficient-of-determination.md) is $1-(1-R^2)(n-1)/(n-2)$.

These are algebraic consistency identities for one specified fit; the mean identity needs no normal-error assumption. A [normal linear model](normal-linear-model-split.md) supplies the usual finite-sample t and F reference distributions. Heteroscedasticity-robust [standard errors](standard-error.md) need not satisfy the displayed F=t-squared relationship to the classical sums-of-squares F statistic. Rounding can create small discrepancies, while different analysed records or a changed model can create larger ones; neither should be silently treated as the same fit.[Value: coefficient matrix, sigma, df, fstatistic and r.squared](summarizing-linear-model-fits-in-the-r-documentation.md)

## ↑ Ancestors (9)

1. [Simple linear regression](simple-linear-regression.md)
2. [Linear regression](linear-regression-split.md)
3. [Normal linear model](normal-linear-model-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/6/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/6/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/6/solution.md)
