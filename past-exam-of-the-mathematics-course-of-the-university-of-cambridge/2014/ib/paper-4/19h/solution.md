<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

For the [normal linear model](../../../../../normal-linear-model.md), differentiating the [ordinary least squares](../../../../../ordinary-least-squares.md) objective gives $X^TX\widehat\beta=X^TY$. Full column [rank](../../../../../rank-one-quadratic-form.md) makes $X^TX$ invertible, so

$$
 \boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad
 \widehat\beta\sim N_p\left(\beta,\sigma^2(X^TX)^{-1}\right).}
$$

The distribution follows because $\widehat\beta=\beta+(X^TX)^{-1}X^T\varepsilon$ is a linear transformation of a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md). Its [expectation](../../../../../expected-value.md) is $\beta$, and direct multiplication gives the displayed [covariance matrix](../../../../../covariance-matrix.md).

Let $H=X(X^TX)^{-1}X^T$, the orthogonal projection onto the design's column space. The [residual sum of squares](../../../../../residual-sum-of-squares.md) is $RSS=\|Y-X\widehat\beta\|^2=Y^T(I-H)Y$. Since $(I-H)X\beta=0$, symmetry and idempotence give $\mathbb E[RSS]=\sigma^2\operatorname{tr}(I-H)=(n-p)\sigma^2$. Thus

$$
 \boxed{\widehat\sigma^2=\frac{RSS}{n-p}}
$$

is an [unbiased estimator](../../../../../unbiased-estimator.md).

For the two independent regressions choose $\beta=(a,b,c,d)^T$. The first $m$ rows of the [design matrix](../../../../../design-matrix.md) are $(1,u_i,0,0)$ and the last $m$ rows are $(0,0,1,w_i)$. The centering conditions and distinct predictors give

$$
 X^TX=\operatorname{diag}(m,S_u,m,S_w),\qquad
 S_u=\sum_i u_i^2>0,\quad S_w=\sum_i w_i^2>0.
$$

It follows that

$$
 \boxed{\widehat a=\overline V,\quad\widehat b=\frac{\sum_i u_iV_i}{S_u},\quad
 \widehat c=\overline Z,\quad\widehat d=\frac{\sum_i w_iZ_i}{S_w}.}
$$

The two estimated slopes are independent [normal random variables](../../../../../gaussian-random-variable.md), as they depend on independent error blocks. Therefore

$$
 \boxed{\widehat b-\widehat d\sim N\left(b-d,\sigma^2\left(\frac1{S_u}+\frac1{S_w}\right)\right).}
$$

For these data use the pooled [residual sum of squares](../../../../../residual-sum-of-squares.md)

$$
 RSS=\sum_i(V_i-\widehat a-\widehat b u_i)^2
 +\sum_i(Z_i-\widehat c-\widehat d w_i)^2,\qquad s^2=\frac{RSS}{2m-4}.
$$

Its scaled value is $\chi^2_{2m-4}$ and is independent of the slope estimates by the permitted normal-model result. Hence the standardized difference has a [Student t-distribution](../../../../../student-s-t-distribution.md) with $2m-4$ degrees of freedom, giving the exact **95 percent confidence interval**

$$
 \boxed{(\widehat b-\widehat d)\ \pm\ t_{2m-4,\,0.975}\,
 s\sqrt{\frac1{S_u}+\frac1{S_w}}.}
$$

Here $t_{\nu,0.975}$ is the 0.975 [quantile](../../../../../quantile-function.md) of that distribution. This is a [confidence interval for the difference of independent regression slopes](../../../../../confidence-interval-for-the-difference-of-independent-regression-slopes.md). As required by the original $p<n$ framework, this specialization needs $m>2$. Distinct predictors alone allow $m=2$, but then the fit is saturated, $RSS=0$ and there are no residual degrees of freedom to estimate the unknown variance or form this interval.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
