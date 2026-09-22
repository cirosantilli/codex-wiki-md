<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With the same squared-error normalization as in Question 2, the [ridge estimator](../../../../../ridge-regression.md) solves

$$
(\widehat a,\widehat\beta_\lambda^R)=\operatorname*{argmin}_{a\in\mathbb R,\ b\in\mathbb R^p}\left\{\frac1{2n}\|Y-a\mathbf1_n-Xb\|_2^2+\frac\lambda2\|b\|_2^2\right\}.
$$

The [unpenalized intercept in ridge regression](../../../../../unpenalized-intercept-in-ridge-regression.md) is $\widehat a=\overline Y$ because the columns of $X$ are centered. Differentiating the remaining quadratic objective gives $(X^TX+n\lambda I_p)\widehat\beta_\lambda^R=X^TY_c$. Since $\lambda>0$, the left matrix is positive definite even when $X$ is rank-deficient. Thus the [closed-form ridge regression estimator](../../../../../closed-form-ridge-regression-estimator.md) is

$$
\boxed{\widehat\beta_\lambda^R=(X^TX+n\lambda I_p)^{-1}X^TY_c=(X^TX+n\lambda I_p)^{-1}X^TY.}
$$

The second equality again uses centering. If the penalty convention is $\lambda\|b\|_2^2/2$ with an unnormalized squared-error term $\|Y_c-Xb\|_2^2/2$, replace $n\lambda$ by $\lambda$ throughout; the limiting assertion is unchanged.

For the full-column-rank case, take a [singular value decomposition](../../../../../singular-value-decomposition.md) $X=UDV^T$ with positive [singular values](../../../../../singular-value.md) $d_1,\ldots,d_p$. The [ordinary least squares](../../../../../ordinary-least-squares.md) estimator, which is the slope [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) in this [normal linear model](../../../../../normal-linear-model.md), and the [ridge regression](../../../../../ridge-regression.md) estimator are respectively

$$
\widehat\beta=\sum_{j=1}^p\frac{u_j^TY}{d_j}v_j,\qquad
\widehat\beta_\lambda^R=\sum_{j=1}^p\frac{d_j}{d_j^2+n\lambda}(u_j^TY)v_j.
$$

Consequently [principal-component shrinkage by ridge regression](../../../../../principal-component-shrinkage-by-ridge-regression.md) multiplies the least-squares coordinate in direction $v_j$ by $d_j^2/(d_j^2+n\lambda)$. **Ridge shrinks most strongly in directions with the smallest [singular values](../../../../../singular-value.md).** These are combinations of predictors that the data distinguish least well.

Near [multicollinearity](../../../../../multicollinearity.md) creates small [singular values](../../../../../singular-value.md), and the factor $1/d_j$ in [ordinary least squares](../../../../../ordinary-least-squares.md) greatly amplifies noise in those directions. Its coefficient variance there is $\sigma^2/d_j^2$, while the ridge variance is

$$
\frac{\sigma^2d_j^2}{(d_j^2+n\lambda)^2},
$$

which is smaller. The price is bias: the expectation of the ridge coordinate is $d_j^2/(d_j^2+n\lambda)$ times the corresponding true coefficient. This [bias-variance tradeoff](../../../../../bias-variance-tradeoff.md) can substantially reduce estimation and prediction error when the poorly identified directions do not contain an excessively large signal. It is not a guarantee of improvement for every coefficient vector. Adding $n\lambda$ to every [eigenvalue](../../../../../eigenvalue.md) also improves the [condition number](../../../../../condition-number.md) of the normal matrix and makes numerical inversion more stable.

To handle every rank and every relation between $n$ and $p$, put $G=X^TX$ and use its [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md). Choose an orthonormal eigenbasis $v_1,\ldots,v_p$ with [eigenvalues](../../../../../eigenvalue.md) $\gamma_j\geq0$, and put $z=X^TY$. Then

$$
\widehat\beta_\lambda^R=\sum_{j=1}^p\frac{v_j^Tz}{\gamma_j+n\lambda}v_j.
$$

If $\gamma_j=0$, then $\|Xv_j\|_2^2=v_j^TGv_j=0$, so $Xv_j=0$ and $v_j^Tz=(Xv_j)^TY=0$. Thus these terms are exactly zero for every positive $\lambda$; there is no divergent component in the [null space](../../../../../kernel-of-a-linear-map.md). Each remaining term converges to $(v_j^Tz/\gamma_j)v_j$. By the definition of the [Moore-Penrose pseudoinverse](../../../../../moore-penrose-inverse.md),

$$
G^+=\sum_{\gamma_j>0}\frac1{\gamma_j}v_jv_j^T,
$$

and therefore

$$
\boxed{\lim_{\lambda\downarrow0}\widehat\beta_\lambda^R=(X^TX)^+X^TY.}
$$

This proves the [vanishing-penalty ridge limit](../../../../../vanishing-penalty-ridge-limit.md) without an invertibility assumption. The limit is the [minimum-norm least-squares solution](../../../../../minimum-norm-least-squares-solution.md): every other least-squares solution differs by a vector in $\ker X$, orthogonal to the displayed solution, and therefore has at least as large a [Euclidean norm](../../../../../euclidean-norm.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
