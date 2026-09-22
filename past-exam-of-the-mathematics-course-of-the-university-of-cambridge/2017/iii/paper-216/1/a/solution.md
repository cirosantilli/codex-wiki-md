<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $a=y_4$ and $b=y_2+y_3$. Dropping factors independent of $\theta$, the [multinomial likelihood](../../../../../../multinomial-likelihood.md) and [uniform prior](../../../../../../uniform-prior.md) give the [posterior density](../../../../../../posterior-density.md)

$$
\pi(\theta\mid y)\propto(2+\theta)^{y_1}\theta^a(1-\theta)^b\mathbf1_{(0,1)}(\theta).
$$

Multiplying this by the stipulated [binomial distribution](../../../../../../binomial-distribution.md) for the [latent variable](../../../../../../latent-variable.md) cancels the factor $(2+\theta)^{y_1}$:

$$
\pi(\theta,z\mid y)\propto\binom{y_1}{z}2^{y_1-z}\theta^{a+z}(1-\theta)^b,
\qquad 0\leq z\leq y_1.
$$

Consequently the two [full conditional distributions](../../../../../../full-conditional-distribution.md) are

$$
\boxed{Z\mid\theta,y\sim\operatorname{Binomial}\!\left(y_1,\frac{\theta}{2+\theta}\right),\qquad
\theta\mid Z=z,y\sim\operatorname{Beta}(a+z+1,b+1).}
$$

Start with $0<\theta_0<1$, sample $Z$ from its [binomial distribution](../../../../../../binomial-distribution.md), then sample a new $\theta$ from its [Beta distribution](../../../../../../beta-distribution.md), and repeat. The [binomial distribution](../../../../../../binomial-distribution.md) can be sampled by adding $y_1$ independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md). For the [Beta distribution](../../../../../../beta-distribution.md), take independent $A\sim\operatorname{Gamma}(a+z+1,1)$ and $B\sim\operatorname{Gamma}(b+1,1)$ and return $A/(A+B)$; integer-shape [gamma distributions](../../../../../../gamma-distribution.md) are sums of independent unit-rate [exponential distributions](../../../../../../exponential-distribution.md). Both shapes are positive even when some observed counts vanish.

Each [Gibbs sampler](../../../../../../gibbs-sampler.md) update preserves the augmented [posterior distribution](../../../../../../bayesian-posterior.md), so its $\theta$ [marginal distribution](../../../../../../marginal-distribution.md) is the required [posterior distribution](../../../../../../bayesian-posterior.md). The positive [full conditional distributions](../../../../../../full-conditional-distribution.md) on the interior allow exploration of the entire support. These iterates are generally dependent; they are not the independent exact draws constructed in the later parts.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
