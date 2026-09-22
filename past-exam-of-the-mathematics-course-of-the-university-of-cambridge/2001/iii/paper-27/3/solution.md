<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [credibility factor](../../../../../credibility-factor.md) is the weight assigned to a particular risk's observed experience when blending it with a population or manual premium. In the [Bühlmann model](../../../../../buhlmann-model.md), the blend is the best affine mean-square predictor, rather than automatically the full [posterior mean](../../../../../posterior-mean.md).

Let $v=\mathbb E[\sigma^2(\theta)]$, the [expected process variance](../../../../../expected-process-variance.md), and assume the displayed second moments are finite. The [law of total expectation](../../../../../law-of-total-expectation.md) gives $\mathbb EX_i=m$. The [law of total variance](../../../../../law-of-total-variance.md) and [law of total covariance](../../../../../law-of-total-covariance.md) give

$$
\boxed{\operatorname{Var}X_i=v+a,\qquad\operatorname{Cov}(X_i,X_j)=a\quad(i\ne j).}
$$

For the second formula, the conditional covariance is zero by conditional independence, while the covariance of the conditional means is $\operatorname{Var}\mu(\theta)=a$, the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md). Likewise

$$
\boxed{\operatorname{Cov}(\mu(\theta),X_i)=a,}
$$

because $\mathbb E[X_i-\mu(\theta)\mid\theta]=0$.

To derive the [Bühlmann credibility premium](../../../../../buhlmann-credibility-premium.md), minimize $\mathbb E[(\mu(\theta)-b_0-\sum_ib_iX_i)^2]$. Differentiating in $b_0$ sets the predictor's mean to $m$. The remaining [normal equations](../../../../../normal-equation.md) are

$$
(vI+a\mathbf1\mathbf1^T)b=a\mathbf1.
$$

For $v>0$, subtracting any two rows forces all $b_i$ to be equal, then gives $b_i=a/(v+na)$. Thus the premium and factor are

$$
\boxed{\widehat\mu=Z\overline X+(1-Z)m,\qquad Z=\frac{na}{na+v}=\frac{n}{n+v/a}.}
$$

The same affine premium predicts $X_{n+1}$: conditional independence makes $\mathbb E[(X_{n+1}-\widehat\mu)^2]=v+\mathbb E[(\mu(\theta)-\widehat\mu)^2]$, so minimizers agree. If $v=0$, every year's amount equals $\mu(\theta)$ almost surely, and $Z=1$ gives the exact risk mean even though the coefficient vector need not be unique.

For fixed $a>0,n$, $\partial Z/\partial v=-na/(na+v)^2<0$. Thus more within-risk variation decreases credibility: individual experience becomes less informative, $Z\to0$ as $v\to\infty$, and the premium tends to $m$. Increasing the number of observed years has the opposite effect.

For numerical estimation from a balanced panel, assume the $k$ risks are independent draws from the same risk population, with comparable exposures, and $n,k\ge2$. Set

$$
\overline X_s=\frac1n\sum_{j=1}^nX_{js},\qquad
\widehat m=\frac1k\sum_{s=1}^k\overline X_s,
$$



$$
\widehat v=\frac1{k(n-1)}\sum_{s=1}^k\sum_{j=1}^n(X_{js}-\overline X_s)^2,\qquad
B=\frac1{k-1}\sum_{s=1}^k(\overline X_s-\widehat m)^2.
$$

Conditionally, each within-risk sample variance has mean $\sigma^2(\theta_s)$; hence $\mathbb E\widehat v=v$. The risk sample means have variance $a+v/n$, so $\mathbb EB=a+v/n$. Therefore $\widetilde a=B-\widehat v/n$ is an unbiased [method of moments](../../../../../method-of-moments-statistics.md) estimate of $a$. For a usable nonnegative variance estimate take $\widehat a=\max(0,\widetilde a)$, noting that this truncation sacrifices exact unbiasedness.

The [balanced-panel method-of-moments credibility](../../../../../balanced-panel-method-of-moments-credibility.md) estimate for risk $s$ is consequently

$$
\boxed{\widehat Z=\frac{n\widehat a}{n\widehat a+\widehat v},\qquad
\widehat\mu_s=\widehat Z\overline X_s+(1-\widehat Z)\widehat m.}
$$

If $\widehat a=0$ and $\widehat v>0$, use zero credibility. If both estimates are zero, the within and between sums of squares are zero and all the observed amounts coincide; any blend gives that same premium. With only one year per risk or only one risk, these within/between estimators are unavailable, so external structural estimates or additional assumptions are necessary.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
