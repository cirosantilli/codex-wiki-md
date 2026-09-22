<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\widehat\beta=(X^TX)^{-1}X^TY$, $H=X(X^TX)^{-1}X^T$, $\widehat y_i=x_i^T\widehat\beta$, and $e_i=y_i-\widehat y_i$. The horizontal axis of the [residual-versus-fitted plot](../../../../../../residual-versus-fitted-plot.md) is $\widehat y_i$, the [fitted values](../../../../../../fitted-values.md), and the vertical axis is $e_i$, the [regression residual](../../../../../../regression-residual.md), in millimetres. Under the [normal linear model](../../../../../../normal-linear-model.md), $\operatorname{Var}(e_i)=\sigma^2(1-h_{ii})$, where $h_{ii}$ is the [regression leverage](../../../../../../regression-leverage.md).

In the [quantile-quantile plot](../../../../../../q-q-plot.md), the vertical values are the ordered [standardized regression residuals](../../../../../../standardized-regression-residual.md)

$$
r_i=\frac{e_i}{s\sqrt{1-h_{ii}}},
$$

and the horizontal values are corresponding theoretical [quantiles](../../../../../../quantile-function.md) $\Phi^{-1}(p_k)$ of the standard [normal distribution](../../../../../../normal-distribution.md), with plotting positions such as $p_k=(k-1/2)/n$. The exact plotting-position convention has little practical effect here. Under Gaussian errors these points should approximately follow a straight line; they are not independent because fitting induces residual correlations.

**The main visible concern is curvature in the conditional mean.** The red smooth in the [residual-versus-fitted plot](../../../../../../residual-versus-fitted-plot.md) descends from positive residuals at low fitted values, becomes negative in the middle, and rises again at high fitted values. This suggests the strictly linear time effects may be inadequate. There is no clear monotone widening of the residual scatter, so strong [heteroscedasticity](../../../../../../heteroscedastic.md) is not apparent. The [quantile-quantile plot](../../../../../../q-q-plot.md) has modest tail deviations and a few labelled observations, but does not show a dramatic departure from [normality](../../../../../../normal-distribution.md). These plots cannot establish [independence](../../../../../../independent-random-variables.md) across days or laboratories; check residuals against day, laboratory, and sampling order as well. A large [coefficient of determination](../../../../../../coefficient-of-determination.md) does not remove the visible mean-model concern.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
