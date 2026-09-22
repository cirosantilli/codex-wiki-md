<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $G=I-H$. Since $GX=0$, the [regression residual](../../../../../../regression-residual.md) vector is $\widehat\varepsilon=G\varepsilon$. A linear transformation of a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) is again [multivariate normal](../../../../../../multivariate-normal-distribution.md), so

$$
\boxed{\widehat\varepsilon\sim N_n(0,\sigma^2G),\qquad G=I-H.}
$$

This is a singular [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) supported on $\ker X^T$, with dimension $n-p$. In particular,

$$
\operatorname{Var}(\widehat\varepsilon_i)=\sigma^2(1-h_{ii}),\qquad
\operatorname{Cov}(\widehat\varepsilon_i,\widehat\varepsilon_j)=-\sigma^2h_{ij}\quad(i\ne j).
$$

Consequently [regression residuals](../../../../../../regression-residual.md) are neither independent nor identically distributed even under the stated model. Their linear constraints include $X^T\widehat\varepsilon=0$, and, if the [design matrix](../../../../../../design-matrix.md) contains an intercept, their sum is zero.

Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) of the residual space. The coordinates of $G\varepsilon$ in that basis are $n-p$ [independent](../../../../../../independent-random-variables.md) $N(0,\sigma^2)$ variables, proving

$$
\frac{Q(\widehat\beta)}{\sigma^2}\sim\chi^2_{n-p},\qquad
s^2=\frac{Q(\widehat\beta)}{n-p}.
$$

For $n>p$, $s^2$ is an [unbiased estimator](../../../../../../unbiased-estimator.md) of $\sigma^2$. Orthogonality of $H$ and $G$ gives zero cross-[covariance](../../../../../../covariance.md), so the [Gaussian](../../../../../../normal-distribution.md) fitted and residual vectors are [independent](../../../../../../independent-random-variables.md). This explains why an appropriate residual-versus-fitted diagnostic has no systematic mean relationship under the model. If $n=p$, no residual information remains for these diagnostics or the variance estimate.

For $h_{ii}<1$, use [standardized regression residuals](../../../../../../standardized-regression-residual.md) $r_i=\widehat\varepsilon_i/[s\sqrt{1-h_{ii}}]$ to account for the different residual [variances](../../../../../../variance-split.md). The diagonal $h_{ii}$ is the [regression leverage](../../../../../../regression-leverage.md); $h_{ii}=1$ makes that residual identically zero and cannot be diagnosed by this standardization. With known $\sigma$, the corresponding individually standardized residual has an exact [standard normal distribution](../../../../../../standard-normal-distribution.md). With estimated $s$, the [internally studentized residual](../../../../../../standardized-regression-residual.md) is not exactly normal or a [Student t-distribution](../../../../../../student-s-t-distribution.md), and the residuals remain correlated; a normal reference plot is a diagnostic approximation.

Plot the [regression residuals](../../../../../../regression-residual.md) or [standardized regression residuals](../../../../../../standardized-regression-residual.md) against [fitted values](../../../../../../fitted-values.md) and each covariate. A persistent curve suggests a misspecified mean, while a fan-shaped spread suggests [heteroscedasticity](../../../../../../heteroscedastic.md); a [scale-location plot](../../../../../../scale-location-plot.md) helps separate these. A [quantile-quantile plot](../../../../../../q-q-plot.md) against normal quantiles checks tails, skewness and possible [regression outliers](../../../../../../regression-outlier.md). Plot residuals against observation order or time to look for unexplained serial patterns, recognizing that projection already induces the displayed residual [covariances](../../../../../../covariance.md). Inspect [regression leverage](../../../../../../regression-leverage.md) together with [Cook's distance](../../../../../../cook-s-distance.md) for [influential observations](../../../../../../influential-observation.md). Such patterns motivate revising the model; absence of a visible pattern does not prove all its assumptions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
