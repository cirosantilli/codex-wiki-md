<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the [Bühlmann model](../../../../../buhlmann-model.md), a latent risk parameter $\Theta$ is drawn from a population distribution. Conditional on $\Theta$, the yearly observations are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md), with [conditional expectation](../../../../../conditional-expectation.md) $m(\Theta)$ and [conditional variance](../../../../../conditional-variance.md) $v(\Theta)$. Define the structural parameters

$$
m=\mathbb E[m(\Theta)],\qquad
v=\mathbb E[v(\Theta)],\qquad
a=\operatorname{Var}(m(\Theta)).
$$

Here $v$ is the [expected process variance](../../../../../expected-process-variance.md), while $a$ is the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md). The [Bühlmann credibility premium](../../../../../buhlmann-credibility-premium.md) is the best affine estimate of $m(\Theta)$ from the observed claims, under [mean squared error](../../../../../mean-squared-error.md). Predicting the next claim gives the same affine estimate: the extra conditional observation noise contributes the constant $v$ to the prediction error.

The [law of total variance](../../../../../law-of-total-variance.md) and [conditional independence](../../../../../conditional-independence.md) give

$$
\operatorname{Var}(X_j)=a+v,\qquad
\operatorname{Cov}(X_i,X_j)=a\quad(i\ne j),\qquad
\operatorname{Cov}(m(\Theta),X_j)=a.
$$

An affine estimate can be written as $\widehat m=m+\sum_{j=1}^n b_j(X_j-m)$: for any chosen $b_j$, optimizing the constant makes its [expected value](../../../../../expected-value.md) equal to $m$. The normal equations for the [linear least-squares projection](../../../../../linear-least-squares-projection.md) are

$$
v b_i+a\sum_{j=1}^n b_j=a,\qquad i=1,\ldots,n.
$$

For $v>0$ they force all $b_i$ to agree, with $b_i=a/(v+na)$. Thus **the credibility factor and premium are**

$$
\boxed{Z=\frac{na}{v+na}=\frac{n}{n+v/a},\qquad
\widehat m=Z\overline X+(1-Z)m,}
\qquad \overline X=\frac1n\sum_{j=1}^nX_j.
$$

The [credibility factor](../../../../../credibility-factor.md) increases with the observation count and between-risk [variance](../../../../../variance-split.md), and decreases with within-risk [variance](../../../../../variance-split.md). If $a=0$, the risk mean is known and $Z=0$; if $v=0$ and $a>0$, one observation reveals it and $Z=1$. If both vanish, the premium is the fixed value $m$ and the factor is immaterial.

In the specified model, the conditional law is a [gamma distribution](../../../../../gamma-distribution.md) with shape $\alpha$ and scale $\theta$. Therefore

$$
m(\theta)=\alpha\theta,\qquad v(\theta)=\alpha\theta^2.
$$

The prior is an [inverse-gamma distribution](../../../../../inverse-gamma-distribution.md) with shape $k$ and scale $\lambda$. To obtain its moments directly, substitute $y=\lambda/\theta$ in the defining integral, obtaining

$$
\mathbb E[\Theta^r]
=\lambda^r\frac{\Gamma(k-r)}{\Gamma(k)},\qquad r<k.
$$

The [Gamma function recurrence](../../../../../gamma-function-recurrence.md) yields

$$
\mathbb E\Theta=\frac{\lambda}{k-1},\qquad
\mathbb E\Theta^2=\frac{\lambda^2}{(k-1)(k-2)},\qquad
\operatorname{Var}(\Theta)=\frac{\lambda^2}{(k-1)^2(k-2)}.
$$

The assumption $k>2$ makes both structural [variances](../../../../../variance-split.md) finite. Hence

$$
m=\frac{\alpha\lambda}{k-1},\qquad
v=\frac{\alpha\lambda^2}{(k-1)(k-2)},\qquad
a=\frac{\alpha^2\lambda^2}{(k-1)^2(k-2)},\qquad
\frac va=\frac{k-1}{\alpha}.
$$

It follows that **the model-specific credibility estimate is**

$$
\boxed{Z=\frac{n\alpha}{n\alpha+k-1},\qquad
\widehat m_{\rm B}
=Z\overline X+(1-Z)\frac{\alpha\lambda}{k-1}
=\frac{\alpha(\lambda+\sum_{j=1}^nX_j)}{k+n\alpha-1}.}
$$

For the [Bayes estimator under squared error loss](../../../../../bayes-estimator-under-squared-error-loss.md), the quantity to estimate is $\alpha\Theta$, so the optimum is its [posterior mean](../../../../../posterior-mean.md). The [likelihood function](../../../../../likelihood-function.md), viewed as a function of $\theta$, is proportional to

$$
\theta^{-n\alpha}\exp\left(-\frac{\sum_jx_j}{\theta}\right).
$$

Multiplication by the prior shows [gamma scale inverse-gamma conjugacy](../../../../../gamma-scale-inverse-gamma-conjugacy.md):

$$
\Theta\mid x_1,\ldots,x_n
\sim\operatorname{InvGamma}\left(k+n\alpha,\lambda+\sum_jx_j\right).
$$

Although the printed hint only mentions integer shapes, the same substitution and [Gamma integral](../../../../../gamma-integral.md) normalize this posterior for every positive real shape, so no integrality of $\alpha$ is needed. Its [posterior mean](../../../../../posterior-mean.md) gives **the Bayesian estimate and comparison**

$$
\boxed{\widehat m_{\rm Bayes}
=\alpha\mathbb E[\Theta\mid X_1,\ldots,X_n]
=\frac{\alpha(\lambda+\sum_{j=1}^nX_j)}{k+n\alpha-1}
=\widehat m_{\rm B}.}
$$

This [exact Bühlmann credibility for gamma claims](../../../../../exact-buhlmann-credibility-for-gamma-claims.md) holds for every observed sample, not merely on average. Here the [posterior mean](../../../../../posterior-mean.md) is affine in the [sample mean](../../../../../sample-mean.md), so the best affine [Bühlmann credibility premium](../../../../../buhlmann-credibility-premium.md) is also the unrestricted [Bayes estimator under squared error loss](../../../../../bayes-estimator-under-squared-error-loss.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
