<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [credibility premium](../../../../../credibility-estimate.md) estimates a risk's expected future claims by combining its own observed experience with a collective or prior mean. In its basic form $Z\overline X+(1-Z)\mu$, the [credibility factor](../../../../../credibility-factor.md) $Z\in[0,1]$ is the weight assigned to individual experience. Larger credibility places less weight on pooling with the population. The amounts below are pure expected-claim premiums; no additional expense or profit loading is specified.

Under [squared-error loss](../../../../../squared-error-loss.md), the posterior risk for estimating the unknown conditional mean $\theta$ by $a$ is

$$
\mathbb E[(\theta-a)^2\mid\boldsymbol X]=\operatorname{Var}(\theta\mid\boldsymbol X)+\left(a-\mathbb E[\theta\mid\boldsymbol X]\right)^2.
$$

Hence the [Bayes estimator under squared error loss](../../../../../bayes-estimator-under-squared-error-loss.md) is the [posterior mean](../../../../../posterior-mean.md). In the equal-year model, [conditional independence](../../../../../conditional-independence.md) makes the likelihood proportional to $\exp[-\sum_{j=1}^n(X_j-\theta)^2/(2\sigma_1^2)]$. Combining it with the normal prior and completing the square gives

$$
\theta\mid\boldsymbol X\sim N(m_n,V_n),\qquad V_n=\left(\frac1{\sigma_2^2}+\frac n{\sigma_1^2}\right)^{-1},\qquad m_n=V_n\left(\frac\mu{\sigma_2^2}+\frac{\sum_jX_j}{\sigma_1^2}\right).
$$

Because $\mathbb E[X_{n+1}\mid\theta]=\theta$, the required estimator is $m_n$; it also equals the predictive mean $\mathbb E[X_{n+1}\mid\boldsymbol X]$. The [normal-normal credibility](../../../../../normal-normal-credibility.md) expression is

$$
\boxed{\widehat\theta=Z\overline X+(1-Z)\mu,\qquad Z=\frac{n\sigma_2^2}{\sigma_1^2+n\sigma_2^2}=\frac n{n+\sigma_1^2/\sigma_2^2}.}
$$

This is exact [Bayesian credibility](../../../../../bayesian-credibility.md), not merely the best linear approximation to a possibly nonlinear [posterior mean](../../../../../posterior-mean.md).

For unequal life counts use the usual exposure model: individual-life losses are conditionally independent with [variance](../../../../../variance-split.md) $v$, and the annual totals are conditionally independent given the same $\theta$. Then

$$
Y_j\mid\theta\ \mathrel{\dot\sim}\ N(m_j\theta,m_jv),\qquad X_j=Y_j/m_j\mid\theta\ \mathrel{\dot\sim}\ N(\theta,v/m_j).
$$

The dot denotes the stipulated normal approximation. The positive exposures $m_j$ are known. Define total past exposure and its experience mean by

$$
W=\sum_{j=1}^nm_j,\qquad\overline X_w=\frac{\sum_jm_jX_j}{W}=\frac{\sum_jY_j}{W}.
$$

The normal log-likelihood has quadratic term $-\sum_jm_j(X_j-\theta)^2/(2v)$. With the prior $N(\mu,\sigma^2)$, [normal-normal conjugacy with unequal exposures](../../../../../normal-normal-conjugacy-with-unequal-exposures.md) gives [posterior variance](../../../../../posterior-variance.md) and mean

$$
V=\left(\frac1{\sigma^2}+\frac Wv\right)^{-1},\qquad m=V\left(\frac\mu{\sigma^2}+\frac{\sum_jY_j}{v}\right).
$$

Therefore the estimated pure premium per life for year $n+1$ has the [normal-normal credibility with unequal exposures](../../../../../normal-normal-credibility-with-unequal-exposures.md) form

$$
\boxed{\widehat\pi_{n+1}=Z_W\overline X_w+(1-Z_W)\mu,\qquad Z_W=\frac{W\sigma^2}{v+W\sigma^2}=\frac W{W+v/\sigma^2}.}
$$

It is also an exact normal-model [Bühlmann–Straub credibility estimate](../../../../../buhlmann-straub-credibility-estimate.md). The individual experience is exposure-weighted: the unweighted mean of the yearly per-life observations would generally discard the different precisions.

For positive $W,v,\sigma^2$, differentiation gives

$$
\frac{\partial Z_W}{\partial\sigma^2}=\frac{Wv}{(v+W\sigma^2)^2}>0,\qquad\frac{\partial Z_W}{\partial v}=-\frac{W\sigma^2}{(v+W\sigma^2)^2}<0.
$$

Thus **increasing the prior [variance](../../../../../variance-split.md) increases credibility**, because greater between-risk heterogeneity makes the collective mean less representative of this risk. **Increasing the individual process [variance](../../../../../variance-split.md) decreases credibility**, because a fixed amount of observed experience becomes noisier. The future exposure supplies no new observation, so it does not enter $Z_W$. It only scales the total premium:

$$
\boxed{\widehat\Pi_{n+1}=m_{n+1}\left[Z_W\frac{\sum_{j=1}^nY_j}{\sum_{j=1}^nm_j}+(1-Z_W)\mu\right].}
$$

The independent-life [variance](../../../../../variance-split.md) scaling is part of the usual exposure interpretation. Without it, a known [variance](../../../../../variance-split.md) $v$ for one life does not determine the [variance](../../../../../variance-split.md) of a total: a common pairwise conditional [covariance](../../../../../covariance.md) $c$ would add $m_j(m_j-1)c$ to $m_jv$. Similarly, cross-year conditional dependence would change the joint likelihood. Those assumptions are implicit in applying the standard credibility model to the final paragraph.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
