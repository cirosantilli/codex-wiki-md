<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [least-squares estimator](../../../../../ordinary-least-squares-estimators.md) minimizes $(Y-Xb)^T(Y-Xb)$. Differentiation gives $X^TX\hat\beta=X^TY$, and the full column [rank](../../../../../rank-one-quadratic-form.md) of $X$ makes $X^TX$ positive definite. Hence

$$
\boxed{\hat\beta=(X^TX)^{-1}X^TY.}
$$

The [fitted values](../../../../../fitted-values.md) are $\hat Y=X\hat\beta=HY$, where the [hat matrix](../../../../../hat-matrix.md) is $H=X(X^TX)^{-1}X^T$. The [regression residuals](../../../../../regression-residual.md) are $\hat\varepsilon=Y-\hat Y=(I-H)Y$. Since $H$ is the [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) onto the column space of $X$, $(I-H)X=0$ and

$$
\boxed{\hat\varepsilon\sim N_n(0,\sigma^2(I-H)).}
$$

This is a singular [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) supported on the $(n-p)$-dimensional orthogonal complement of the column space: its components are generally correlated. The equality $\hat Y=X\hat\beta$ puts the fitted vector in that column space, while $X^T\hat\varepsilon=0$ expresses [fitted-residual orthogonality](../../../../../fitted-residual-orthogonality.md). No residual component lies in an explanatory direction that could improve the least-squares fit.

For the calibration model, write $R_i$ for a reading and $a_i$ for the known amount. The first fit assumes $R_i=\alpha+\beta a_i+\varepsilon_i$ with independent $N(0,\sigma^2)$ errors. Its [residual-versus-fitted plot](../../../../../residual-versus-fitted-plot.md) has systematic changes in group means and an increasing within-group spread. These suggest both a nonlinear mean relationship and [heteroscedasticity](../../../../../heteroscedastic.md), rather than the random scatter expected from a satisfactory [normal linear model](../../../../../normal-linear-model.md).

The [Box–Cox transformation](../../../../../box-cox-transformation.md) plot is a profile [log-likelihood](../../../../../log-likelihood.md) for the power parameter $\lambda$. Its maximum is near $0.94$; the horizontal line gives an approximate 95% [likelihood-ratio confidence interval](../../../../../likelihood-ratio-confidence-interval.md), which excludes the untransformed value $1$. Since affine rescaling of the response does not change the fitted mean space, fitting the raw power $R_i^{0.94}$ is equivalent to using $(R_i^{0.94}-1)/0.94$ with an intercept. The second model is

$$
R_i^{0.94}=\alpha+\beta a_i+\varepsilon_i,\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Its residual spread is more even, but observation 17 has a conspicuously negative residual near $-9.95$. This motivates checking for an [outlier](../../../../../outlier.md) or recording error. The third fit omits that observation; omission should be justified by that investigation, since choosing exclusions from residuals can affect inference. Some group pattern still remains, so the transformation alone does not certify a perfect model.

At an amount of $3$ nanograms, the third fit predicts the transformed mean

$$
\hat m=-3.62509+30.87295(3)=88.99376.
$$

Simply applying the inverse power gives $\hat m^{1/0.94}=118.5187$. The requested expected reading needs [bias correction after an inverse transformation](../../../../../bias-correction-after-an-inverse-transformation.md), since $\mathbb E[g(Z)]\ne g(\mathbb E[Z])$ for nonlinear $g$. With $q=1/0.94$ and $s=2.832$, a second-order [Taylor expansion](../../../../../taylor-expansion.md) gives

$$
\boxed{\widehat{\mathbb E[R\mid a=3]}\simeq\hat m^q+\frac12q(q-1)\hat m^{q-2}s^2=118.5227.}
$$

Here the correction uses the residual variance, rather than the variance of the estimated fitted mean. The power-transformed Gaussian model is an approximation for positive readings; the fitted mean is over 31 residual standard deviations above zero, so the negative tail has negligible effect on this local approximation. The ordinary inverse-transformed prediction is therefore essentially $118.52$ at the displayed precision.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
