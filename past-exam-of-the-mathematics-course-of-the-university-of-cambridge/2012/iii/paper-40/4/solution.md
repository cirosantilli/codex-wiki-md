<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [credibility estimate](../../../../../credibility-estimate.md) blends the risk's own [sample mean](../../../../../sample-mean.md) with a population or prior [expected value](../../../../../expected-value.md). In the basic equal-exposure form it is $Z\overline X+(1-Z)\mu$, where the [credibility factor](../../../../../credibility-factor.md) $Z\in[0,1]$ is the weight attached to the individual experience. More data ordinarily increase that weight; greater within-risk variation relative to between-risk variation reduces it.

Write $m(\theta)=\mu(\theta)$ for the conditional claim [expected value](../../../../../expected-value.md), keeping $\mu$ for the prior-level parameter. Normalization of the [probability density function](../../../../../probability-density-function.md) gives

$$
q(\theta)=\int_0^\infty p(x)e^{-\theta x}\,dx.
$$

At interior points of its finite domain, [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) yields

$$
q'(\theta)=-\int_0^\infty xp(x)e^{-\theta x}\,dx,
\qquad
\boxed{m(\theta)=-\frac{q'(\theta)}{q(\theta)}.}
$$

This is an instance of the [exponential-family derivative identities](../../../../../exponential-family-derivative-identities.md) for natural parameter $-\theta$. The minus sign is present in the PDF and is lost in the converted TeX. The [conditional variance](../../../../../conditional-variance.md) is likewise $(\log q)''(\theta)$.

Differentiate the log of the [natural conjugate prior](../../../../../natural-conjugate-prior.md):

$$
\frac{\pi'(\theta)}{\pi(\theta)}
=-k\frac{q'(\theta)}{q(\theta)}-k\mu
=k\bigl(m(\theta)-\mu\bigr).
$$

Integrate on a compact subinterval and then let its endpoints approach those of the parameter interval. The prescribed vanishing of the prior density eliminates the boundary term. Since $m(\theta)\geq0$, [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) justifies the limit of its expectation, and the identity gives

$$
\boxed{\mathbb E_\pi[m(\Theta)]=\mu.}
$$

In particular the assumed proper prior and boundary conditions themselves establish this first-moment integrability.

For $T=\sum_{i=1}^nx_i$ and $\overline x=T/n$, [conditional independence](../../../../../conditional-independence.md) makes the [likelihood function](../../../../../likelihood-function.md) proportional to $q(\theta)^{-n}e^{-\theta T}$. Multiplication by the [prior distribution](../../../../../prior-probability.md) gives the [Bayesian posterior](../../../../../bayesian-posterior.md)

$$
\pi(\theta\mid\mathbf x)\propto q(\theta)^{-(k+n)}e^{-\theta(k\mu+T)}.
$$

Thus this is a [conjugate prior](../../../../../conjugate-prior.md) family, with updated parameters

$$
\boxed{k_n=k+n,\qquad \mu_n=\frac{k\mu+T}{k+n}.}
$$

The integration-by-parts calculation for the [posterior mean](../../../../../posterior-mean.md) also needs vanishing posterior boundary values. Here that property can be checked, rather than assumed. Let $a,b$ be the essential lower and upper endpoints of the claim support. Every nondegenerate tilted claim law has $a<m(\theta)<b$, so the established prior mean satisfies $a<\mu<b$. Supported observations have $\overline x\in[a,b]$; hence $a<\mu_n<b$. At a finite parameter endpoint the prior's vanishing forces $q(\theta)\to\infty$, because its exponential factor has a finite positive limit; the increased power $q^{-k_n}$ makes the posterior vanish there too. At $\theta\to+\infty$, choose $a<d<\mu_n$ with positive base-measure mass below $d$. Then $q(\theta)\geq C e^{-d\theta}$ and the unnormalized posterior is at most $C^{-k_n}e^{-k_n(\mu_n-d)\theta}\to0$. At $\theta\to-\infty$, choose $\mu_n<d<b$ with positive mass above $d$ to obtain the corresponding bound $C^{-k_n}e^{k_n(d-\mu_n)\theta}\to0$. These bounds also ensure posterior propriety at infinite endpoints. This is the [endpoint control for a Laplace-family conjugate posterior](../../../../../endpoint-control-for-a-laplace-family-conjugate-posterior.md).

Apply the previous score integration to the [Bayesian posterior](../../../../../bayesian-posterior.md). The [natural conjugate credibility identity](../../../../../natural-conjugate-credibility-identity.md) is

$$
\boxed{\mathbb E[m(\Theta)\mid\mathbf x]=\mu_n
=\frac n{n+k}\overline x+\frac k{n+k}\mu.}
$$

Thus **$Z=n/(n+k)$** is the [credibility factor](../../../../../credibility-factor.md). This is an exact [posterior mean](../../../../../posterior-mean.md), rather than an affine approximation to one.

For the specific shape-two [gamma distribution](../../../../../gamma-distribution.md), take

$$
\boxed{p(x)=x,\qquad q(\theta)=\theta^{-2},\qquad \theta>0.}
$$

Then $m(\theta)=2/\theta$ and $\operatorname{Var}(X\mid\theta)=2/\theta^2$. The [gamma rate gamma conjugacy](../../../../../gamma-rate-gamma-conjugacy.md) prior is

$$
\boxed{\pi(\theta)=\frac{(k\mu)^{2k+1}}{\Gamma(2k+1)}\theta^{2k}e^{-k\mu\theta},\qquad \theta>0,}
$$

that is, $\Theta\sim\operatorname{Gamma}(2k+1,\text{rate }k\mu)$. Its normalizing constant in the notation of the question is $c(\mu,k)=\Gamma(2k+1)/(k\mu)^{2k+1}$. The [gamma distribution](../../../../../gamma-distribution.md) density vanishes at both zero and infinity for $k>0$. The posterior has shape $2k+2n+1$ and rate $k\mu+T$, so its conditional-mean [posterior mean](../../../../../posterior-mean.md) is again $(k\mu+T)/(k+n)$.

For the last calculation, [gamma distribution](../../../../../gamma-distribution.md) integration gives

$$
\mathbb E[\Theta^{-1}]=\frac{k\mu}{2k}=\frac\mu2,
\qquad
\mathbb E[\Theta^{-2}]=\frac{(k\mu)^2}{2k(2k-1)}.
$$

The second identity requires the printed $k>1/2$. Therefore the [expected process variance](../../../../../expected-process-variance.md) and [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md), denoted by $a,b$ in this question, are

$$
\boxed{a=\mathbb E[2/\Theta^2]=\frac{k\mu^2}{2k-1},\qquad
b=\operatorname{Var}(2/\Theta)=\frac{\mu^2}{2k-1}.}
$$

Consequently $a/b=k$, and the [Bühlmann credibility factor](../../../../../credibility-factor.md) agrees with the exact Bayesian weight:

$$
\boxed{Z=\frac n{n+k}=\frac n{n+a/b}.}
$$

This is the [exact Bühlmann credibility for gamma claims](../../../../../exact-buhlmann-credibility-for-gamma-claims.md), expressed using the reciprocal rate as the random scale. The symbols $a,b$ here are the process and between-risk [variances](../../../../../variance-split.md), respectively; their roles should not be interchanged when comparing with other notation for the [Bühlmann model](../../../../../buhlmann-model.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
