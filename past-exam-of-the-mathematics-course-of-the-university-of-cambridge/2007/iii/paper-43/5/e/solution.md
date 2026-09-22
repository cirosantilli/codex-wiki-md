<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

`library(mgcv)` loads the fitting package; `gam` fits a Gaussian [generalised additive model](../../../../../../generalized-additive-model.md) with the printed identity link. The smooth specification `s(x, bs="cr")` uses a penalized [cubic regression spline](../../../../../../cubic-regression-spline.md). This is a finite-dimensional smooth basis, rather than a full interpolating [spline](../../../../../../spline-mathematics.md) with a free value at all $401$ observations. The fitted model is

$$
\boxed{Y_i=\beta_0+f(x_i)+\varepsilon_i,\qquad\varepsilon_i\text{ independent }N(0,\sigma^2),\qquad\sum_{i=1}^{401}f(x_i)=0.}
$$

Here $f(x)=\sum_{r=1}^q\theta_rB_r(x)$ in the centred cubic regression-spline basis, with its curvature penalized through $\lambda\int(f'')^2$. The intercept is estimated separately. In the displayed fit the smooth test space has rank $9$, consistent with nine smooth coefficients after the centring constraint, while penalization lowers its effective dimension.

The intercept estimate is $-0.13241$, with [standard error](../../../../../../standard-error.md) $0.05426$, $t=-2.44$ and $p=0.0151$. Because the smooth is centred over the observations, the intercept is the overall fitted average, not necessarily the fitted response at $x=0$. Its test compares this average with zero. The significance-code legend maps progressively smaller $p$-values to stars; stars are an annotation, not an effect-size measure.

The smooth has $8.237$ [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md), displaying substantial nonlinearity: a centred purely linear term would use one. `Est.rank=9` reports the rank used for its approximate significance calculation. The $p$-value below $2\times10^{-16}$ is very strong evidence that the mean depends on $x$, against a zero smooth term. It does not mean the fitted curve is the exact generating function, or that lack of fit has been tested. The total effective dimension including the intercept is $1+8.237=9.237$.

The [adjusted coefficient of determination](../../../../../../adjusted-coefficient-of-determination.md) $R^2$ of $0.983$ and [deviance](../../../../../../exponential-family-deviance.md) explained of $98.4\%$ indicate that nearly all variation about the response mean is explained. For this Gaussian model, [deviance](../../../../../../exponential-family-deviance.md) explained is $1-\operatorname{RSS}/\operatorname{SST}$. The scale estimate $0.96737$ estimates residual [variance](../../../../../../variance-split.md), corresponding to a residual standard deviation about $0.984$. The [GCV](../../../../../../generalized-cross-validation.md) score $0.99018$ is the prediction-oriented criterion used for smoothing selection, not a probability. It is consistent with the reported scale and effective dimension: $0.96737\times401/(401-9.237)\simeq0.99018$.

In the PDF's plot, the solid curve is the estimated centred smooth $f(x)$, and the dashed curves show pointwise uncertainty around that smooth, rather than [prediction intervals](../../../../../../prediction-interval.md) for new noisy responses. The label `s(x,8.24)` gives its rounded [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md). The rug marks the observed [covariate](../../../../../../covariate.md) locations. Reading the endpoints gives

$$
\boxed{-10\le x\le10.}
$$

The smooth is increasing with an almost flat middle and one inflection, resembling a cubic. A simpler model to investigate is ordinary Gaussian [polynomial regression](../../../../../../polynomial-regression.md)

$$
\boxed{Y_i=\beta_0+\beta_1x_i+\beta_2x_i^2+\beta_3x_i^3+\varepsilon_i.}
$$

It uses four mean coefficients rather than about nine effective ones. The apparent near-odd shape also makes $\beta_0+\beta_3x^3$ a plausible further reduction, but the linear and quadratic terms should be checked rather than discarded solely from the picture. The figure suggests this alternative; it does not supply coefficients or establish the true simulation model.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
