<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Minimizing the [residual sum of squares](../../../../../residual-sum-of-squares.md) $\|Y-Xb\|^2$ gives the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) $X^TX\widehat\beta=X^TY$. Since the [design matrix](../../../../../design-matrix.md) has full [column rank](../../../../../column-rank.md), $X^TX$ has a [matrix inverse](../../../../../matrix-inverse.md), so

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad
\widehat\beta\sim N_p\bigl(\beta,\sigma^2(X^TX)^{-1}\bigr).}
$$

The [sampling distribution](../../../../../sampling-distribution.md) follows because a linear transformation of a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) is again a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md). Its [expectation](../../../../../expected-value.md) is $\beta$, and its [covariance matrix](../../../../../covariance-matrix.md) is $\sigma^2(X^TX)^{-1}X^TX(X^TX)^{-1}=\sigma^2(X^TX)^{-1}$.

The [hat matrix](../../../../../hat-matrix.md) is $H=X(X^TX)^{-1}X^T$. It is the [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) onto the [column space](../../../../../column-space.md) of $X$: $H^T=H$, $H^2=H$ and $HX=X$. Thus the [regression residuals](../../../../../regression-residual.md) are $\widehat\varepsilon=(I-H)Y$, with

$$
\operatorname{Cov}(\widehat\varepsilon,\widehat Y)
=\sigma^2(I-H)H=0,\qquad
\operatorname{Cov}(\widehat\varepsilon,\widehat\beta)
=\sigma^2(I-H)X(X^TX)^{-1}=0.
$$

This is [fitted-residual orthogonality](../../../../../fitted-residual-orthogonality.md). The vectors are jointly normal, so [independence of uncorrelated jointly normal variables](../../../../../independence-of-uncorrelated-jointly-normal-variables.md) strengthens both zero-[covariance](../../../../../covariance.md) statements to [independence](../../../../../independent-random-variables.md).

For the quadratic [linear regression](../../../../../linear-regression-split.md), the columns of the [design matrix](../../../../../design-matrix.md) are $1,x,x^2$. The replicated design gives

$$
X^TX=\begin{pmatrix}30&0&20\\0&20&0\\20&0&20\end{pmatrix},\qquad
\boxed{\operatorname{Cov}\begin{pmatrix}\widehat\alpha\\\widehat\beta\\\widehat\gamma\end{pmatrix}
=\sigma^2\begin{pmatrix}1/10&0&-1/10\\0&1/20&0\\-1/10&0&3/20\end{pmatrix}.}
$$

For $v(x)=(1,x,x^2)^T$, the [variance of a fitted regression mean](../../../../../variance-of-a-fitted-regression-mean.md) is $\sigma^2v(x)^T(X^TX)^{-1}v(x)$, hence

$$
\boxed{\operatorname{Var}(\widehat\alpha+\widehat\beta x+\widehat\gamma x^2)
=\frac{\sigma^2}{20}(2-3x^2+3x^4).}
$$

Writing $u=x^2\in[0,1]$, this is the quadratic $(\sigma^2/20)(2-3u+3u^2)$. Its [derivative](../../../../../derivative.md) vanishes at $u=1/2$; it decreases before that point and increases afterwards. Therefore the **maximum** is $\sigma^2/10$ at $x=-1,0,1$, and the **minimum** is $\sigma^2/16$ at $x=\pm1/\sqrt2$.

At $100^\circ\mathrm C$, $x=0$ and the expected yield is $\alpha$. The unbiased residual [variance](../../../../../variance-split.md) estimate is $s^2=2.43/(30-3)=0.09$. By [Cochran's theorem](../../../../../cochran-s-theorem.md), $27s^2/\sigma^2\sim\chi^2_{27}$ independently of $\widehat\alpha$, giving the [Student t confidence interval](../../../../../student-t-confidence-interval.md)

$$
\boxed{\alpha\in\left[\widehat\alpha-t_{27,0.975}\sqrt{0.009},\;
\widehat\alpha+t_{27,0.975}\sqrt{0.009}\right]
\simeq[\widehat\alpha-0.19465,\widehat\alpha+0.19465].}
$$

The interval estimates the expected yield, so it uses the [variance of a fitted regression mean](../../../../../variance-of-a-fitted-regression-mean.md) without an additional future-observation error term. The supplied summary determines the half-width but does not give a numerical value of $\widehat\alpha$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
