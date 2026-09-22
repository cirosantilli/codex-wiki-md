<h1 id="10j/solution">Solution</h1>

↑ **Parent:** [10J](../10j.md)

Write $R_j=I-P_{-j}$. Minimizing the residual sum of squares first over the coefficients of $X_{-j}$ reduces the problem to minimizing $\|R_jY-bR_jX_j\|^2$. Full column rank ensures $R_jX_j\ne0$. Thus the [partial regression](../../../../../partial-regression.md) formula and its [variance](../../../../../variance-split.md) are

$$
\boxed{\widehat\beta_j=\frac{X_j^TR_jY}{X_j^TR_jX_j},\qquad\operatorname{var}(\widehat\beta_j)=\frac{\sigma^2}{X_j^TR_jX_j}.}
$$

This uses $R_j^T=R_j=R_j^2$ and the isotropic error [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2I$.

Since the span of $X_k$ is contained in the column space of $X_{-j}$, [orthogonal projection](../../../../../orthogonal-projection.md) onto the latter removes at least as much squared norm. Consequently

$$
X_j^TR_jX_j\leq\|X_j\|^2-\frac{(X_k^TX_j)^2}{\|X_k\|^2},
$$

and inversion proves the requested lower bound. Full rank makes the denominator positive.

Adding $c\mathbf1_n$ to column $j\geq2$ leaves the column space unchanged. Every old fitted vector is reproduced by keeping all slopes unchanged and replacing the [regression intercept](../../../../../regression-intercept.md) by $\widehat\beta_1-c\widehat\beta_j$. Uniqueness of the [ordinary least squares estimators](../../../../../ordinary-least-squares-estimators.md) then proves that slope $j$ is unchanged. In particular all columns can be centered by such changes. Applying the previous projection argument to the centered design proves the bound with $X_j-\bar X_j\mathbf1_n$ and $X_k-\bar X_k\mathbf1_n$; the normalized inner product is now the usual [sample correlation](../../../../../sample-correlation-coefficient.md).

Each reported coefficient test is the two-sided [Student's t-test](../../../../../student-s-t-test.md) of $H_0:\beta_j=0$ against $H_1:\beta_j\ne0$, conditional on the other predictors. Under the null, $\widehat\beta_j/(\widehat\sigma\sqrt{(X^TX)^{-1}_{jj}})$ has a [Student's t-distribution](../../../../../student-s-t-distribution.md) with $100-3=97$ degrees of freedom. At five percent the intercept is significant, but neither individual test slope is. The final [F-test](../../../../../f-test.md) compares the full model against an intercept-only model: $H_0:\beta_{\rm Maths}=\beta_{\rm Stats}=0$. It has $(2,97)$ degrees of freedom and rejects at five percent, since its $p$-value is $0.003166$. Thus the predictors jointly explain variation, without strong evidence separating their individual conditional effects.

The two test predictors have [sample correlation](../../../../../sample-correlation-coefficient.md) $0.9371630$, although each has only moderate correlation with the final exam response. The [variance inflation factor](../../../../../variance-inflation-factor.md) is $1/(1-0.9371630^2)\simeq8.22$. Their nearly shared direction produces substantial [multicollinearity](../../../../../multicollinearity.md), inflating the individual slope standard errors. The joint [F-test](../../../../../f-test.md) can detect this common predictive direction even though either coefficient, given the other, has a large $p$-value.

## ↑ Ancestors (10)

1. [10J](../10j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
