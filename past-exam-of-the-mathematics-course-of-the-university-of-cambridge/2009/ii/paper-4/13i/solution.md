<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

Put $M=X^TX$, which is positive definite because $X$ has [full column rank](../../../../../full-column-rank.md). The log [likelihood](../../../../../likelihood-function.md) differs from $-\|Y-X\beta\|^2/(2\sigma^2)$ by a term independent of $\beta$. Differentiation gives the normal equations $M\widehat\beta=X^TY$, hence

$$
\boxed{\widehat\beta=M^{-1}X^TY,\qquad
\widehat\beta\sim N_p(\beta,\sigma^2M^{-1}).}
$$

The distribution follows by writing $\widehat\beta=\beta+M^{-1}X^T\varepsilon$ and applying the [linear transformation](../../../../../linear-map.md) rule for a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md).

Let $s=\sigma^2$ and $R=\|Y-X\widehat\beta\|^2$. [Orthogonality](../../../../../orthogonal-vectors.md) of the residual to the columns of $X$ gives the exact decomposition

$$
\|Y-X\beta\|^2=R+(\beta-\widehat\beta)^TM(\beta-\widehat\beta).
$$

The prior is density proportional to $s^{-1}$ with respect to $d\beta\,ds$. Thus the joint [posterior distribution](../../../../../bayesian-posterior.md) is

$$
\boxed{\pi(\beta,s\mid X,Y)\propto
s^{-n/2-1}\exp\left[-\frac{R+(\beta-\widehat\beta)^TM(\beta-\widehat\beta)}{2s}\right].}
$$

Completing the quadratic identifies

$$
\boxed{\beta\mid s,X,Y\sim N_p(\widehat\beta,sM^{-1}).}
$$

The sampling distribution treats the true $\beta$ as fixed and varies the data, whereas the conditional posterior fixes the observed data and distributes $\beta$. Their [covariance](../../../../../covariance.md) formulas agree, but their centres and their interpretations differ.

For a new row vector $x^*$, let $h^*=x^*M^{-1}(x^*)^T$ and suppose its new error is independent. With known $\sigma^2$, the maximum-likelihood plug-in prediction uses mean $x^*\widehat\beta$ and noise [variance](../../../../../variance-split.md) $\sigma^2$, while a calibrated frequentist prediction must account for the estimator: $y^*-x^*\widehat\beta\sim N(0,\sigma^2(1+h^*))$. If [variance](../../../../../variance-split.md) is estimated, the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is $R/n$, whereas the exact frequentist prediction pivot uses $\widehat s=R/(n-p)$ and has [Student t-distribution](../../../../../student-s-t-distribution.md) with $n-p$ degrees of freedom.

In the Bayesian calculation, integrating $\beta$ first gives $y^*\mid s,X,Y\sim N(x^*\widehat\beta,s(1+h^*))$. Integrating $\beta$ out of the joint posterior gives $s\mid X,Y\sim\operatorname{InvGamma}((n-p)/2,R/2)$. For $\nu=n-p$, integration of the predictive normal against this [inverse-gamma distribution](../../../../../inverse-gamma-distribution.md) has density proportional to

$$
\int_0^\infty s^{-(\nu+1)/2-1}\exp\left[-\frac{R+(y^*-x^*\widehat\beta)^2/(1+h^*)}{2s}\right]ds
\propto\left[1+\frac{(y^*-x^*\widehat\beta)^2}{R(1+h^*)}\right]^{-(\nu+1)/2}.
$$

The substitution $t=[R+(y^*-x^*\widehat\beta)^2/(1+h^*)]/(2s)$ reduces the integral to a [Gamma function](../../../../../gamma-function.md). Normalizing identifies the [Student t-distribution](../../../../../student-s-t-distribution.md), giving

$$
\boxed{y^*\mid X,Y\sim t_{n-p}\left(x^*\widehat\beta,\ \sqrt{\frac{R}{n-p}(1+h^*)}\right),}
$$

where the second parameter is a scale, not its [variance](../../../../../variance-split.md). These Bayesian intervals coincide with the usual exact Gaussian-regression [prediction intervals](../../../../../prediction-interval.md) for this prior, although their probability interpretations differ. Posterior propriety requires $R>0$ and $n>p$; the former holds almost surely under the nondegenerate Gaussian model. Prediction of the noiseless conditional mean omits the added one in $1+h^*$.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
