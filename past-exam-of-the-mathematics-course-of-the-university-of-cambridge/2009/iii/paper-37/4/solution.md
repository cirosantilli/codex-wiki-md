<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let the [Bühlmann–Straub model](../../../../../buhlmann-straub-model.md) structural parameters be

$$
m_0=\mathbb E[\mu(\Theta)],\qquad a=\operatorname{Var}(\mu(\Theta)),\qquad v=\mathbb E[\sigma^2(\Theta)],\qquad W=\sum_{j=1}^nm_j.
$$

Here $a$ is the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md) and $v$ is the [expected process variance](../../../../../expected-process-variance.md). Assume the structural second moments are finite and the exposures $m_j$ are positive, as required by this least-squares problem. Write $A=\sum_ja_j$. Conditional independence separates the squared prediction error into squared conditional bias and conditional variance. The [law of total expectation](../../../../../law-of-total-expectation.md) gives

$$
\mathbb E\!\left[\left(\mu(\Theta)-a_0-\sum_ja_jX_j\right)^2\right]=a(1-A)^2+\bigl((1-A)m_0-a_0\bigr)^2+v\sum_j\frac{a_j^2}{m_j}.
$$

Indeed, conditional on $\Theta$, the prediction has mean $a_0+A\mu(\Theta)$ and variance $\sigma^2(\Theta)\sum_ja_j^2/m_j$; there are no cross-covariances because the annual observations are conditionally independent.

For fixed slope coefficients the optimal intercept is $a_0=(1-A)m_0$. For fixed sum $A$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
A^2=\left(\sum_j\frac{a_j}{\sqrt{m_j}}\sqrt{m_j}\right)^2\le W\sum_j\frac{a_j^2}{m_j},
$$

with equality when $a_j=A m_j/W$. Thus the remaining minimization is the scalar quadratic

$$
a(1-A)^2+\frac vW A^2.
$$

Differentiation gives $A=Z=aW/(aW+v)$. In the nondegenerate case $a,v>0$, the quadratic is strictly convex and the equality condition determines the unique slope coefficients. The **[Bühlmann–Straub credibility factor](../../../../../buhlmann-straub-credibility-factor.md) and premium** are therefore

$$
\boxed{Z=\frac{aW}{aW+v},\qquad a_j=\frac{am_j}{aW+v},\qquad a_0=(1-Z)m_0,}
$$

and

$$
\boxed{\widehat\mu_{\rm cred}=Z\overline X_w+(1-Z)m_0,\qquad\overline X_w=\frac{\sum_jm_jX_j}{W}.}
$$

This derives the [Bühlmann–Straub credibility estimate](../../../../../buhlmann-straub-credibility-estimate.md) from its minimization criterion. Increasing exposure increases the weight on experience; increasing process noise decreases it. No exposure for year $n+1$ appears because the estimate concerns the expected claim per car, not the variance of next year's observed average.

The degenerate cases have a direct interpretation. If $a=0$ and $v>0$, the unknown conditional mean is the known constant $m_0$, so take $Z=0$. If $v=0$ and $a>0$, each observation already equals $\mu(\Theta)$ almost surely, so $Z=1$ gives exact prediction. If both vanish, all observations and the target equal $m_0$ almost surely; use the constant predictor rather than the undefined ratio $0/0$.

In the approximate normal model, $\mu(\Theta)=\Theta$, $m_0=\mu$, $\operatorname{Var}(\Theta)=a$, and $\sigma^2(\Theta)=v$. Substitution into the derived [credibility estimate](../../../../../credibility-estimate.md) gives

$$
\boxed{\widehat\mu_{\rm cred}=\frac{a\sum_jm_jX_j+v\mu}{aW+v}.}
$$

We now derive, rather than assume, the [Bayes estimator under squared error loss](../../../../../bayes-estimator-under-squared-error-loss.md). For positive $a,v$, the [likelihood](../../../../../likelihood-function.md) and [normal distribution](../../../../../normal-distribution.md) prior give a posterior density proportional to

$$
\exp\!\left[-\frac12\left\{\frac{(\theta-\mu)^2}{a}+\frac1v\sum_jm_j(X_j-\theta)^2\right\}\right].
$$

The coefficient of $\theta^2$ is $1/a+W/v$, and the coefficient in the linear term is $\mu/a+\sum_jm_jX_j/v$. Completing the square proves the [normal-normal conjugacy with unequal exposures](../../../../../normal-normal-conjugacy-with-unequal-exposures.md) formula

$$
\Theta\mid X_1,\ldots,X_n\sim N(m_*,V_*),\qquad V_*=(1/a+W/v)^{-1}=\frac{av}{v+aW},
$$

with

$$
m_*=\frac{\mu/a+\sum_jm_jX_j/v}{1/a+W/v}=\frac{v\mu+a\sum_jm_jX_j}{v+aW}.
$$

For any decision $d$, the posterior [quadratic loss](../../../../../squared-error-loss.md) is

$$
\mathbb E[(\Theta-d)^2\mid X]=V_*+(m_*-d)^2.
$$

Its unique minimizer is the [posterior mean](../../../../../posterior-mean.md) $d=m_*$. Hence **the Bayesian and credibility estimates coincide exactly in this normal model**:

$$
\boxed{\widehat\mu_{\rm Bayes}=m_*=\widehat\mu_{\rm cred}.}
$$

The reason is that the posterior mean is already affine in the observations, so restricting prediction to affine functions loses nothing. In the general [Bühlmann–Straub model](../../../../../buhlmann-straub-model.md), the posterior mean need not be affine; the [credibility estimate](../../../../../credibility-estimate.md) is then only the best affine squared-error predictor. The zero-variance limits of the normal formulas agree with the degenerate cases above.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
