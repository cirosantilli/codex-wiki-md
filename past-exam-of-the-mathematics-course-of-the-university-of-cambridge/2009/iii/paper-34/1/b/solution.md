<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [log-likelihood](../../../../../../log-likelihood.md) in the [normal linear model](../../../../../../normal-linear-model.md), up to an additive constant, is

$$
\ell(\beta,\sigma^2)=-\frac n2\log\sigma^2-\frac1{2\sigma^2}\|Y-X\beta\|^2.
$$

Full column rank makes $X^TX$ [positive-definite](../../../../../../positive-definite-bilinear-form.md), so minimizing the residual sum of squares gives the [normal equations](../../../../../../normal-equation.md) $X^TX\widehat\beta=X^TY$. Maximizing over $\sigma^2$ afterward gives the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad\widehat\sigma^2=\frac1n\|Y-X\widehat\beta\|^2.}
$$

The residual sum of squares is positive almost surely because $n-p>0$ and $\sigma^2>0$, so this maximization has an interior [variance](../../../../../../variance-split.md) solution almost surely. The first estimator is a linear Gaussian statistic with mean $\beta$ and [covariance](../../../../../../covariance.md) $\sigma^2(X^TX)^{-1}$, giving

$$
\boxed{\widehat\beta\sim N_p\bigl(\beta,\sigma^2(X^TX)^{-1}\bigr).}
$$

Let $P_X=X(X^TX)^{-1}X^T$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the design column space, and let $A=I-P_X$. This is a symmetric idempotent matrix of rank $n-p$. Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) for its range and collect its columns in $L$, so $A=LL^T$, $L^TL=I_{n-p}$ and $L^TX=0$. Then

$$
L^TY\sim N_{n-p}(0,\sigma^2I),\qquad\|Y-X\widehat\beta\|^2=Y^TAY=\|L^TY\|^2.
$$

The definition of the [chi-squared distribution](../../../../../../chi-squared-distribution.md) therefore gives

$$
\boxed{\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p},\qquad\widehat\sigma^2\sim\frac{\sigma^2}{n}\chi^2_{n-p}.}
$$

The maximum-likelihood denominator is $n$; the unbiased residual-variance estimator uses $n-p$.

Finally put $B=(X^TX)^{-1}X^T$. It has rank $p$ and $BA=0$, because $X^T(I-P_X)=0$. Part (a) implies that $BY=\widehat\beta$ is independent of $Y^TAY=n\widehat\sigma^2$. Multiplication by a fixed constant preserves independence, so the [normal linear model maximum-likelihood sampling distributions](../../../../../../normal-linear-model-maximum-likelihood-sampling-distributions.md) satisfy

$$
\boxed{\widehat\beta\text{ and }\widehat\sigma^2\text{ are independent}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
