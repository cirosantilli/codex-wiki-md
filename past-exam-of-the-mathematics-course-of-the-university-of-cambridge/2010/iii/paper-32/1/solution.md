<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $G=X^TX$ and $H=XG^{-1}X^T$. The [rank of a matrix](../../../../../matrix-rank.md) assumption makes $G$ invertible, and $H$ is the [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) onto the column space of the [design matrix](../../../../../design-matrix.md). The [Gaussian likelihood](../../../../../gaussian-likelihood.md) has [log-likelihood](../../../../../log-likelihood.md)

$$
\ell(b,v)=-\frac n2\log(2\pi v)-\frac{\|Y-Xb\|^2}{2v},\qquad v>0.
$$

Minimizing the squared [Euclidean norm](../../../../../euclidean-norm.md) gives the [ordinary least squares](../../../../../ordinary-least-squares.md) normal equations $G\widehat\beta=X^TY$. Maximizing over $v$ then gives the [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\beta=G^{-1}X^TY,\qquad \widehat\sigma^2=\frac{\mathrm{RSS}}n,\qquad \mathrm{RSS}=Y^T(I-H)Y.}
$$

The divisor for the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) of the [variance](../../../../../variance-split.md) is $n$, whereas the unbiased residual [variance](../../../../../variance-split.md) estimate is $s^2=\mathrm{RSS}/(n-p)$. The exceptional event $\mathrm{RSS}=0$ has probability zero under the [Gaussian linear model](../../../../../normal-linear-model.md) with $\sigma^2>0$; on that event the [likelihood](../../../../../likelihood-function.md) is unbounded as $v\downarrow0$.

For the joint [sampling distribution](../../../../../sampling-distribution.md), write $\widehat\beta-\beta=G^{-1}X^T\epsilon$ and $Y-X\widehat\beta=(I-H)\epsilon$. Their cross-[covariance matrix](../../../../../covariance-matrix.md) vanishes because $X^T(I-H)=0$. These two vectors are jointly [multivariate normal](../../../../../multivariate-normal-distribution.md), so they are [independent random variables](../../../../../independent-random-variables.md). The residual [orthogonal projection](../../../../../orthogonal-projection.md) has rank $n-p$, hence the standard [chi-squared distribution](../../../../../chi-squared-distribution.md) result gives

$$
\boxed{\widehat\beta\sim N_p(\beta,\sigma^2G^{-1}),\qquad \frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p},\qquad \widehat\beta\ \text{and}\ \widehat\sigma^2\ \text{independent}.}
$$

Thus these two displayed marginal laws, with their [independence](../../../../../independent-random-variables.md), specify the full joint distribution.

The [quadratic form](../../../../../quadratic-form.md)

$$
\frac{(\widehat\beta-\beta)^TG(\widehat\beta-\beta)}{\sigma^2}
$$

has a [chi-squared distribution](../../../../../chi-squared-distribution.md) with $p$ degrees of freedom and is independent of $\mathrm{RSS}/\sigma^2$. Their ratio therefore supplies the exact [F-distribution](../../../../../f-distribution.md) pivot

$$
T(\beta)=\frac{(\widehat\beta-\beta)^TG(\widehat\beta-\beta)/p}{\mathrm{RSS}/(n-p)}\sim F_{p,n-p}.
$$

If $f_{1-\alpha}$ is the $(1-\alpha)$ quantile of that [F-distribution](../../../../../f-distribution.md), inversion gives the [normal linear-model confidence ellipsoid](../../../../../normal-linear-model-confidence-ellipsoid.md)

$$
\boxed{C_{1-\alpha}(Y)=\{b\in\mathbb R^p:(\widehat\beta-b)^TG(\widehat\beta-b)\le p s^2 f_{1-\alpha}\}.}
$$

For every $\beta$ and every $\sigma^2>0$, the probability that this [confidence set](../../../../../confidence-region.md) contains $\beta$ is exactly $1-\alpha$. To test the [null hypothesis](../../../../../null-hypothesis.md), reject precisely when $\beta_0$ lies outside this [confidence ellipsoid](../../../../../confidence-ellipsoid.md), equivalently when $T(\beta_0)>f_{1-\alpha}$. Under the [null hypothesis](../../../../../null-hypothesis.md) the rejection probability is exactly $\alpha$, independent of the unknown [variance](../../../../../variance-split.md).

For the numerical calculation, the second column of the [design matrix](../../../../../design-matrix.md) sums to zero and its sum of squares is $60$. Direct calculation from the observations gives

$$
G=\begin{pmatrix}9&0\\0&60\end{pmatrix},\qquad X^TY=\begin{pmatrix}0\\30\end{pmatrix},\qquad Y^TY=22.
$$

Consequently the [ordinary least squares](../../../../../ordinary-least-squares.md) estimate, [residual sum of squares](../../../../../residual-sum-of-squares.md) and unbiased residual [variance](../../../../../variance-split.md) are

$$
\widehat\beta=\begin{pmatrix}0\\1/2\end{pmatrix},\qquad \mathrm{RSS}=22-(X^TY)^TG^{-1}(X^TY)=22-15=7,\qquad s^2=7/7=1.
$$

The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) of the [variance](../../../../../variance-split.md) is instead $7/9$. At the proposed null value the [F-distribution](../../../../../f-distribution.md) statistic is

$$
\boxed{T(0)=\frac{15/2}{7/7}=7.5>4.74.}
$$

Therefore **reject the null hypothesis at the 5% level**. The relevant critical value has $2$ numerator and $7$ residual degrees of freedom.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
