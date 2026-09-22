<h1 id="3/3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the usual normalization that $\varepsilon_t$ is mean-zero unit-[variance](../../../../../../../variance-split.md) [white noise](../../../../../../../white-noise.md) orthogonal to the past, and extend $\phi(\nu),\sigma(\nu)$ periodically in $\nu$. A nondegenerate causal [periodic autoregressive model of order one](../../../../../../../periodic-autoregressive-model-of-order-one.md) requires $|\prod_{\nu=1}^T\phi(\nu)|<1$. Write $V_\nu=\gamma_\nu(0)$, with season indices understood modulo $T$.

For $h\geq1$, multiply the recursion by $X_{nT+\nu-h}$ and use orthogonality of the current innovation to the past. The [periodic Yule-Walker equations](../../../../../../../periodic-yule-walker-equations.md) are

$$
\boxed{\gamma_\nu(h)=\phi(\nu)\gamma_{\nu-1}(h-1),\qquad h\geq1.}
$$

At lag zero, expansion of the squared recursion gives

$$
\boxed{V_\nu=\phi(\nu)^2V_{\nu-1}+\sigma(\nu)^2.}
$$

In particular, $\gamma_\nu(1)=\phi(\nu)V_{\nu-1}$, so an equivalent [variance](../../../../../../../variance-split.md) equation is $V_\nu=\phi(\nu)\gamma_\nu(1)+\sigma(\nu)^2$. Negative lags are obtained from the given symmetry $\gamma_\nu(-h)=\gamma_{\nu+h}(h)$.

Replacing [covariances](../../../../../../../covariance.md) by their sample versions gives

$$
\boxed{\widehat\phi(\nu)=\frac{\widehat\gamma_\nu(1)}{\widehat\gamma_{\nu-1}(0)},\qquad
\widehat\sigma(\nu)=\left(\widehat\gamma_\nu(0)-\frac{\widehat\gamma_\nu(1)^2}{\widehat\gamma_{\nu-1}(0)}\right)^{1/2}.}
$$

Take the nonnegative scale and require a positive estimated predecessor [variance](../../../../../../../variance-split.md). Using matched seasonal sample [covariance](../../../../../../../covariance.md) matrices makes the quantity under the square root nonnegative by [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md); with unmatched [covariance](../../../../../../../covariance.md) estimates one can instead fit seasonal [ordinary least squares](../../../../../../../ordinary-least-squares.md) and use the nonnegative residual [variance](../../../../../../../variance-split.md). [Statistical consistency](../../../../../../../consistency-statistics.md) of the [covariance](../../../../../../../covariance.md) estimates gives [statistical consistency](../../../../../../../consistency-statistics.md) of these plug-in estimators. If the driving noise [variance](../../../../../../../variance-split.md) were not normalized to $1$, the equations would identify $\sigma(\nu)^2\operatorname{Var}(\varepsilon_t)$, not the two scales separately.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
