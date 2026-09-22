<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a common intercept and laboratory-specific slopes in the [normal linear model](../../../../../../normal-linear-model.md). With $t_i$ denoting days and $I_{Bi},I_{Ci}$ the [indicator variables](../../../../../../indicator-variable.md) for laboratories B and C, the [design matrix](../../../../../../design-matrix.md) has row $x_i^T=(1,t_i,t_iI_{Bi},t_iI_{Ci})$, and

$$
Y_i=\beta_0+\beta_At_i+\delta_Bt_iI_{Bi}+\delta_Ct_iI_{Ci}+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The [interaction terms](../../../../../../interaction-term.md) change slopes, without introducing laboratory-specific intercepts. Thus the estimated daily growth rates are

$$
\boxed{\widehat b_A=10.1404,\qquad\widehat b_B=10.1404+5.0770=15.2174,\qquad\widehat b_C=10.1404-3.1296=7.0108}
$$

in millimetres per day, with fitted common intercept $0.6464$ mm. The [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md) are $30-4=26$. The usual unbiased error [variance](../../../../../../variance-split.md) estimate is the square of the residual [standard error](../../../../../../standard-error.md):

$$
\boxed{s^2=15.09^2=227.7081\ \mathrm{mm}^2.}
$$

The small difference from $5921.7/26\approx227.758$ arises from rounding the [standard error](../../../../../../standard-error.md) to two decimal places; the latter uses the more precise [residual sum of squares](../../../../../../residual-sum-of-squares.md) supplied later. A [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) would instead divide that [residual sum of squares](../../../../../../residual-sum-of-squares.md) by $30$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
