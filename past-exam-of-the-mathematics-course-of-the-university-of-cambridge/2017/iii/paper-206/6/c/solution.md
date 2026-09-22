<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first binned [empirical semivariogram](../../../../../../empirical-semivariogram.md) rises strongly through the displayed distances, approximately quadratically, with no visible sill. The spatial data plot shows higher depth at larger $y$. A stationary residual [covariance](../../../../../../covariance.md) should not be asked to explain that deterministic drift.

For a model $Z(s)=m(s)+W(s)$ with stationary zero-mean residual field, each raw squared difference has [expectation](../../../../../../expected-value.md)

$$
\frac12\mathbb E[Z(s_i)-Z(s_j)]^2=\gamma_W(\|s_i-s_j\|)+\frac12[m(s_i)-m(s_j)]^2.
$$

With linear drift $m(x,y)=\beta_0+\beta_1y$, the added term is $\tfrac12\beta_1^2(y_i-y_j)^2$. Its average within distance bins can grow with separation, producing the shape seen in the first plot. The [empirical semivariogram](../../../../../../empirical-semivariogram.md) uses half the average squared difference over the pairs in each bin, so removing only a common intercept does not remove this drift contribution.

The formula `depth ~ y` estimates and removes a linear drift before computing a residual [empirical semivariogram](../../../../../../empirical-semivariogram.md). The second graph levels off near $0.47$ with a fitted zero nugget and a finite scale, making the Gaussian residual [covariance](../../../../../../covariance.md) a plausible working model. **Estimate the drift and fit spatial dependence to residuals rather than the raw depth differences.** Estimated residuals are not the true errors, so their [semivariogram](../../../../../../semivariogram.md) has estimation effects; sparse long-distance bins are also noisy. These graphs support the model but do not establish stationarity or isotropy.

The subpart refers to `svgm` and `svgm2`, while the code calls the objects `smvg` and `smvg2`. Also the printed code omits the line that fits `gauss.model2` before plotting or using it. The supplied output must be interpreted as the result of that missing residual-variogram fit, rather than as an executable complete script.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
