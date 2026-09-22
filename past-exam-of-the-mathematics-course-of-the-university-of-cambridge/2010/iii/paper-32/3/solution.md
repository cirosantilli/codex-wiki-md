<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In a [linear regression](../../../../../linear-regression-split.md) model, a large number of predictors or nearly dependent columns of the [design matrix](../../../../../design-matrix.md) can make some [eigenvalues](../../../../../eigenvalue.md) of $G=X^TX$ small. The [ordinary least squares](../../../../../ordinary-least-squares.md) estimate has [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2G^{-1}$, so these directions have large [variance](../../../../../variance-split.md), even though the estimator is unbiased. [Ridge regression](../../../../../ridge-regression.md) reduces this [variance](../../../../../variance-split.md) by shrinking the estimate towards zero, at the cost of introducing [bias](../../../../../bias-of-an-estimator.md). This [bias-variance tradeoff](../../../../../bias-variance-tradeoff.md) can improve the [mean squared error](../../../../../mean-squared-error.md) when the signal is not too large in the shrunken directions.

For the usual preprocessing with a [regression intercept](../../../../../regression-intercept.md), separate the constant column from the predictors and leave the intercept unpenalized. Subtract the [sample mean](../../../../../sample-mean.md) from the response and from each nonconstant predictor, then divide each centered predictor column by its positive scale, for example its [Euclidean norm](../../../../../euclidean-norm.md). Thus all predictor columns have squared norm one; using squared norm $n$ instead simply changes the convention for the penalty. Centering is performed on the slope columns, not on the constant column. A full-rank design containing an intercept retains full rank on its centered slope columns. A model without an intercept should retain its specified mean structure unless an intercept is deliberately introduced.

Let $Z$ be the resulting scaled, centered slope [design matrix](../../../../../design-matrix.md), let $Y_c$ be the centered response, and let $b$ denote the coefficients in these standardized coordinates. The [ridge regression](../../../../../ridge-regression.md) problem is

$$
\min_{b\in\mathbb R^q}\bigl\{\|Y_c-Zb\|^2+\lambda\|b\|^2\bigr\},\qquad \lambda>0.
$$

Here $q$ is the number of slopes; it is one less than the original number of columns when a constant column was present. The [gradient](../../../../../gradient.md) of this objective is $2(Z^TZ+\lambda I)b-2Z^TY_c$. Its [Hessian matrix](../../../../../hessian-matrix.md) is a [positive-definite matrix](../../../../../positive-definite-matrix.md), giving the unique [closed-form ridge regression estimator](../../../../../closed-form-ridge-regression-estimator.md)

$$
\boxed{\widehat b_\lambda^R=(Z^TZ+\lambda I)^{-1}Z^TY_c.}
$$

The [regression intercept](../../../../../regression-intercept.md) in the original coordinates is recovered as $\widehat a=\overline Y-\sum_j\overline X_j\widehat b_j/s_j$, and the original slopes are $\widehat\beta_j=\widehat b_j/s_j$, where $s_j$ is the scale used for column $j$. This is the [unpenalized intercept in ridge regression](../../../../../unpenalized-intercept-in-ridge-regression.md) convention. For a fixed full-rank coefficient design written simply as $X$, with response $Y$ and coefficient $\beta$, the same formula reads

$$
\boxed{\widehat\beta_\lambda^R=(X^TX+\lambda I)^{-1}X^TY.}
$$

The risk comparison below first uses the fixed coefficient coordinates in which this quadratic penalty is imposed, and then addresses reversal of the scaling.

Assume at least one penalized coefficient, zero-mean errors with [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2I$, and $\sigma^2>0$. No [normal distribution](../../../../../normal-distribution.md) assumption is needed for this [mean squared error](../../../../../mean-squared-error.md) calculation. Put $G=X^TX$ and $A_\lambda=(G+\lambda I)^{-1}$. The [covariance and bias of a ridge regression estimator](../../../../../covariance-and-bias-of-a-ridge-regression-estimator.md) follow directly from its linear expression:

$$
\mathbb E\widehat\beta_\lambda^R-\beta=-\lambda A_\lambda\beta,\qquad
\operatorname{Cov}(\widehat\beta_\lambda^R)=\sigma^2A_\lambda G A_\lambda.
$$

For the centered slope model, the response errors have [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2C$, where $C=I-\mathbf1\mathbf1^T/n$. Since $CZ=Z$, the same coefficient [covariance matrix](../../../../../covariance-matrix.md) formula still holds with $X=Z$.

By the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md), write $G=Q\operatorname{diag}(d_1,\ldots,d_q)Q^T$, with $Q$ orthogonal and every $d_j>0$, and put $\gamma=Q^T\beta$. The [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md) now gives

$$
\mathcal R(\lambda)=\mathbb E\|\widehat\beta_\lambda^R-\beta\|^2
=\sum_{j=1}^q\frac{\lambda^2\gamma_j^2+\sigma^2d_j}{(d_j+\lambda)^2},\qquad
\mathcal R(0)=\sigma^2\sum_{j=1}^q\frac1{d_j}.
$$

The expression at $\lambda=0$ is the [ordinary least squares](../../../../../ordinary-least-squares.md) [mean squared error](../../../../../mean-squared-error.md). Its right derivative is

$$
\mathcal R'(0)=-2\sigma^2\sum_{j=1}^q\frac1{d_j^2}<0.
$$

Therefore, for every fixed coefficient vector, **all sufficiently small positive penalties strictly improve mean squared error**.

An explicit sufficient choice follows by subtracting the [ordinary least squares](../../../../../ordinary-least-squares.md) risk term by term:

$$
\mathcal R(\lambda)-\mathcal R(0)
=\sum_{j=1}^q\frac{\lambda\left(\lambda\gamma_j^2-2\sigma^2-\lambda\sigma^2/d_j\right)}{(d_j+\lambda)^2}.
$$

Since $\gamma_j^2\le\|\beta\|^2$, every summand is negative whenever

$$
\boxed{\lambda>0,\qquad\lambda\|\beta\|^2<2\sigma^2.}
$$

When $\beta=0$, every positive penalty works. This is a pointwise result: the permitted penalty may depend on the true coefficient vector. A fixed positive penalty cannot improve risk for all arbitrarily large signals, because its squared [bias](../../../../../bias-of-an-estimator.md) grows quadratically with the signal. The same distinction appears in [uniform directional risk improvement by ridge regression](../../../../../uniform-directional-risk-improvement-by-ridge-regression.md) and [unbounded directional risk of fixed ridge shrinkage](../../../../../unbounded-directional-risk-of-fixed-ridge-shrinkage.md). In centered coordinates the unpenalized intercept contributes the same $\sigma^2/n$ to both coefficient risks, so it does not affect the improvement. Reversing a fixed predictor scaling measures coefficient error with a fixed [positive-definite matrix](../../../../../positive-definite-matrix.md) $W$ instead of the [identity matrix](../../../../../identity-matrix.md). For this weighted loss the squared [bias](../../../../../bias-of-an-estimator.md) still has derivative zero at $\lambda=0$, while the [variance](../../../../../variance-split.md) term has derivative

$$
-2\sigma^2\operatorname{tr}(WG^{-2})<0.
$$

The inequality follows because $\operatorname{tr}(WG^{-2})=\operatorname{tr}(G^{-1}WG^{-1})>0$. Thus sufficiently small penalties also improve the original-coordinate [mean squared error](../../../../../mean-squared-error.md), though the explicit sufficient bound above was for the unweighted coordinates. Recovering an uncentered intercept adds a fixed nonnegative quadratic form to the slope loss, and its sample-mean error is uncorrelated with the centered slope errors, so the same weighted argument applies. A model with only an unpenalized intercept gives identical estimators. If the noise [variance](../../../../../variance-split.md) were zero, the strict improvement assertion would fail; positive noise [variance](../../../../../variance-split.md) is essential.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
