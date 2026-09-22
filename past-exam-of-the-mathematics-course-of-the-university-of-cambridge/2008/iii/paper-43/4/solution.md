<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [credibility estimate](../../../../../credibility-estimate.md) combines a risk's own observed experience with a collective or prior mean, in the form $Z\widehat\mu_{\mathrm{experience}}+(1-Z)\mu_{\mathrm{collective}}$. The [credibility factor](../../../../../credibility-factor.md) $Z\in[0,1]$ is the weight given to that risk's experience. [Bayesian credibility](../../../../../bayesian-credibility.md) starts with a prior distribution for a latent risk parameter, updates it using observations, and estimates the conditional risk mean by its [Bayesian posterior](../../../../../bayesian-posterior.md) expected value under [squared-error loss](../../../../../squared-error-loss.md). In conjugate models this posterior mean can have exactly the displayed credibility form.

For the unequal policy exposures, define

$$
M=\sum_{i=1}^k m_i,\qquad s=\sum_{i=1}^k x_i.
$$

Conditional independence of the [binomial distribution](../../../../../binomial-distribution.md) observations gives the likelihood, up to a factor not depending on $\theta$,

$$
L(\theta)\propto\prod_{i=1}^k\theta^{x_i}(1-\theta)^{m_i-x_i}
=\theta^s(1-\theta)^{M-s}.
$$

Multiplication by the [Beta distribution](../../../../../beta-distribution.md) prior therefore gives [Beta-binomial conjugacy](../../../../../beta-binomial-conjugacy.md):

$$
\boxed{\theta\mid x_1,\ldots,x_k\sim
\operatorname{Beta}(\alpha+s,\beta+M-s).}
$$

Both posterior parameters are positive, since $0\le s\le M$ and the prior parameters are positive.

The conditional target is $\mu(\theta)=m_{k+1}\theta$. To verify the quadratic-loss rule directly, for any proposed estimate $d$ and observed data $\mathcal D$,

$$
\mathbb E[(d-\mu(\theta))^2\mid\mathcal D]
=(d-\mathbb E[\mu(\theta)\mid\mathcal D])^2
+\operatorname{Var}(\mu(\theta)\mid\mathcal D).
$$

The variance term does not depend on $d$, so the unique [Bayes estimator under squared error loss](../../../../../bayes-estimator-under-squared-error-loss.md) is the posterior mean. Applying the beta mean formula gives

$$
\boxed{\widehat\mu_{k+1}
=m_{k+1}\frac{\alpha+s}{\alpha+\beta+M}.}
$$

It is also the posterior expected future claim count, by the [tower property of conditional expectation](../../../../../law-of-total-expectation.md).

Let $p_0=\alpha/(\alpha+\beta)$ be the collective prior claim probability and $\widehat p=s/M$ the observed claims per policy. Then

$$
\frac{\alpha+s}{\alpha+\beta+M}
=\frac{M}{M+\alpha+\beta}\frac{s}{M}
+\frac{\alpha+\beta}{M+\alpha+\beta}\frac{\alpha}{\alpha+\beta}.
$$

Therefore the [exact beta-binomial credibility with unequal exposures](../../../../../exact-beta-binomial-credibility-with-unequal-exposures.md) is

$$
\boxed{\widehat\mu_{k+1}
=Z\left(m_{k+1}\frac{s}{M}\right)
+(1-Z)\left(m_{k+1}\frac{\alpha}{\alpha+\beta}\right),
\qquad Z=\frac{M}{M+\alpha+\beta}.}
$$

The individual experience must be weighted by exposure: $s/M$ is the policy-weighted frequency, not the unweighted average of $x_i/m_i$ when the $m_i$ differ. The factor multiplies next-year expected counts after scaling both component probabilities by $m_{k+1}$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
