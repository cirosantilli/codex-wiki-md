<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Where the [moment-generating function](../../../../../moment-generating-function.md) $M_Y(t)=\mathbb E e^{tY}$ is finite in a neighborhood of zero, define the [cumulant-generating function](../../../../../cumulant-generating-function.md) $\kappa_Y(t)=\log M_Y(t)$ and the $r$th [cumulant](../../../../../cumulant.md) by $\kappa_r(Y)=\kappa_Y^{(r)}(0)$. Differentiation gives

$$
\kappa_Y'(0)=\frac{M_Y'(0)}{M_Y(0)}=\mathbb EY,
\qquad
\kappa_Y''(0)=M_Y''(0)-M_Y'(0)^2=\operatorname{Var}Y,
$$

since $M_Y(0)=1$. Thus **the first two cumulants are the mean and variance**.

Conditional on $N=n$, independence gives $\mathbb E(e^{tT}\mid N=n)=M_V(t)^n$. Summing over the [Poisson distribution](../../../../../poisson-distribution.md) yields

$$
M_T(t)=e^{-\nu}\sum_{n=0}^{\infty}\frac{(\nu M_V(t))^n}{n!}
=\exp\{\nu(M_V(t)-1)\}.
$$

Hence the [compound Poisson cumulants](../../../../../compound-poisson-cumulants.md) give

$$
\boxed{\kappa_T(t)=\nu(M_V(t)-1),\qquad
\mathbb ET=\nu\mathbb EV,\qquad\operatorname{Var}T=\nu\mathbb EV^2.}
$$

For the moment statements, finite second moments suffice even when a moment-generating function does not exist near zero: conditioning gives $\operatorname{Var}T=\mathbb EN\operatorname{Var}V+\operatorname{Var}N(\mathbb EV)^2=\nu\mathbb EV^2$. This distinguishes the raw second moment from the variance of an individual claim.

For a single flood, the [law of total expectation](../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../law-of-total-variance.md) similarly give

$$
\mathbb ES_i=\lambda\mu,\qquad\operatorname{Var}S_i=\lambda(\sigma^2+\mu^2).
$$

Condition on the number of floods and apply the same laws once more. All floods have these moments and are independent of $M$, so the annual total satisfies

$$
\boxed{\mathbb ES=\nu\lambda\mu,\qquad
\operatorname{Var}S=\nu\bigl[\lambda(\sigma^2+\mu^2)+\lambda^2\mu^2\bigr].}
$$

The additional $\nu\lambda^2\mu^2$ term is the variation in the number of entire flood clusters; it would be lost by treating individual claims as an ordinary Poisson stream.

For the annual count $N=\sum_{i=1}^M N_i$, its [probability generating function](../../../../../probability-generating-function.md) is

$$
\boxed{G_N(z)=\mathbb E(e^{\lambda(z-1)M})=
\exp\{\nu(e^{\lambda(z-1)}-1)\}.}
$$

This is the [nested Poisson flood count](../../../../../nested-poisson-flood-count.md). Differentiating, or conditioning on $M$, gives $\mathbb EN=\nu\lambda$ and $\operatorname{Var}N=\nu\lambda(1+\lambda)$. Thus **$N$ is not Poisson when $\nu,\lambda>0$**, since its variance exceeds its mean. If either parameter is zero it is identically zero, a degenerate Poisson distribution.

Let $K_i$ be the number of valid claims in flood $i$. Independent validity marking gives $K_i\mid N_i\sim\operatorname{Binomial}(N_i,1-p)$. Its generating function is

$$
\mathbb E z^{K_i}=\exp\{\lambda[p+(1-p)z-1]\}
=\exp\{\lambda(1-p)(z-1)\},
$$

so [Poisson thinning](../../../../../poisson-thinning.md) gives **$\boxed{K_i\sim\operatorname{Poisson}(\lambda(1-p))}$**. With validity independent also of claim amount, each claim contributes expected paid amount $(1-p)\mu$. Therefore **the annual expected payment is $\boxed{\nu\lambda(1-p)\mu}$**. The independent-mark assumption is needed for this multiplication; a size-dependent invalidity rule would require the joint expected value of amount and validity instead.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
