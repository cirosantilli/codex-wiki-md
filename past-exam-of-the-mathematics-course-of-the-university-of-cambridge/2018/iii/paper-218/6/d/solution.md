<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\lambda$ denote the effective penalty in the Gaussian squared-error objective. With the loss normalization used in [the glmnet documentation](https://glmnet.stanford.edu/articles/glmnet.html), alpha zero gives [ridge regression](../../../../../../ridge-regression.md):

$$
\boxed{\min_{\beta_0,\beta_1,\beta_2}\left\{\frac1{2n}\sum_{i=1}^n(y_i-\beta_0-\beta_1x_{i1}-\beta_2x_{i2})^2+\frac\lambda2(\beta_1^2+\beta_2^2)\right\},\qquad\lambda\geq0.}
$$

The intercept is fitted separately and unpenalized. The constant column supplied by model.matrix is not an additional penalized slope; glmnet excludes zero-variance predictor columns. Centering and the stated predictor norms make the two slope columns already standardized under the divisor-$n$ convention.

Let $X_s$ consist of those two columns, $z=y-\bar y\mathbf1$, and $G=X_s^TX_s$. Minimizing over the intercept gives $\widehat\beta_0=\bar y$, and the [closed-form ridge regression estimator](../../../../../../closed-form-ridge-regression-estimator.md) under this normalization is

$$
\widehat\beta_\lambda=(G+n\lambda I_2)^{-1}X_s^Tz.
$$

Thus the right-hand limit in the plotted log-$\lambda$ coordinate is $\lambda\to\infty$, giving

$$
\boxed{\widehat\beta_{1,\lambda}\to0,\qquad\widehat\beta_{2,\lambda}\to0.}
$$

The left-hand limit is $\lambda\to0$, giving the unpenalized full-model slopes

$$
\boxed{\widehat\beta_{1,\lambda}\to1.8663,\qquad\widehat\beta_{2,\lambda}\to-0.7209.}
$$

The plotted curves are these two slopes. If the objective is instead written as unnormalized RSS plus a quadratic penalty, its penalty coefficient is $n\lambda$, not $\lambda$.

There is also a software response-scale convention to distinguish from this mathematical parameterization. The [Gaussian fitting engine](https://raw.githubusercontent.com/cran/glmnet/master/src/glmnetpp/include/glmnetpp_bits/elnet_driver/gaussian.hpp) divides a supplied penalty by the response standard deviation $s_y=\sqrt{n^{-1}\sum_i(y_i-\bar y)^2}$ while fitting a standardized response, then rescales the coefficients. For pure ridge with these already standardized predictors, this corresponds to effective $\lambda=\lambda_{\mathrm{API}}/s_y$ in the displayed objective. Such a fixed positive rescaling of the horizontal parameter for the observed dataset does not change either asymptote. The fixed-penalty variance formulas below refer to $\lambda$ in the displayed mathematical objective.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
