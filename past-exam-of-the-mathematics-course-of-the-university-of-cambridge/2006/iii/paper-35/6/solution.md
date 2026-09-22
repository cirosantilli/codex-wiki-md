<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Markov jump process](../../../../../markov-jump-process.md), considered up to its explosion time, is an [adapted](../../../../../adapted-process.md) càdlàg piecewise-constant process whose conditional future law given $\mathcal F_t$ depends only on its current state. Describe its rates by an off-diagonal kernel $q(x,dy)$ with finite total rate $q(x,E)$. In state $x$ the [holding time](../../../../../holding-time.md) has the [exponential distribution](../../../../../exponential-distribution.md) with this rate, followed by a destination distributed as $q(x,dy)/q(x,E)$; a zero-rate state is absorbing. Its [Markov jump-process generator](../../../../../markov-jump-process-generator.md) acts by

$$
Qf(x)=\int_E[f(y)-f(x)]q(x,dy).
$$

The [Markov property](../../../../../markov-property.md) must hold relative to the specified [filtration](../../../../../filtration-probability-theory.md), not merely the natural [filtration](../../../../../filtration-probability-theory.md): future-revealing information could change the jump compensator.

Let $\mu$ count jumps, marked by their destination states. For this [jump measure of a Markov jump process](../../../../../jump-measure-of-a-markov-jump-process.md), the [predictable](../../../../../predictable-process.md) compensator is

$$
\nu(ds,dy)=q(X_{s-},dy)ds.
$$

The compensated random-measure theorem says that a [predictable](../../../../../predictable-process.md) $H(s,y)$ with $\mathbb E\int_0^t\int|H|d\nu<\infty$ gives a true [martingale](../../../../../martingale-split.md)

$$
(H*(\mu-\nu))_t=\int_{(0,t]\times E}H(s,y)(\mu-\nu)(ds,dy).
$$

The same statement holds locally when that expected integrability is obtained after localization. The compensator identity applied to $\mathbf1_A\mathbf1_{(s,t]}H$, for $A\in\mathcal F_s$, shows that each increment has zero [conditional expectation](../../../../../conditional-expectation.md). Taking $H(s,y)=f(y)-f(X_{s-})$ gives the generator [local martingale](../../../../../local-martingale.md) $f(X_t)-f(X_0)-\int_0^t Qf(X_s)ds$. This states the integrability conditions in the [compensated jump-measure local martingale](../../../../../compensated-jump-measure-local-martingale.md) result explicitly.

For the birth-process claim first take the customary fixed initial state $X_0=i$. Write $N_t=X_t-i$, $\Lambda_t=\int_0^t\lambda(X_s)ds$ and $a=e^\theta-1$. The compensator of $N$ is $\Lambda$, whose integrand may equivalently use $X_{s-}$ because jump times have zero Lebesgue measure. A birth multiplies $e^{\theta X}$ by $e^\theta$, so the jump product rule gives

$$
\boxed{dM_t=aM_{t-}\bigl(dN_t-\lambda(X_{t-})dt\bigr),\qquad M_0=e^{\theta i}.}
$$

For an explicit localization, stop at $\tau_n=\inf\{t:X_t\ge n\}\wedge n$ with $n>i$. Up to that time the statewise rates are bounded by the maximum of the finitely many rates below $n$, the jump count is bounded, and $M$ and its compensated-integral integrand are bounded on the finite stopped horizon. The compensated-measure theorem therefore makes each stopped process a true [martingale](../../../../../martingale-split.md). The times increase to the explosion lifetime (or infinity if there is no explosion), proving **$M$ is a [local martingale](../../../../../local-martingale.md) on $[0,\zeta)$ for every real $\theta$**.

Now suppose $\lambda(j)\le C$ uniformly. For $C>0$, propose candidate births at the times of a rate-$C$ [Poisson process](../../../../../poisson-process.md), accepting each with probability $\lambda(X_{s-})/C$ using fresh independent uniform marks. While the state is fixed, [Poisson thinning](../../../../../poisson-thinning.md) gives a [holding time](../../../../../holding-time.md) with the required [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$; accepted births have exactly the prescribed law. Thus there can be no explosion, and the true birth count $N_T$ is stochastically dominated by a [Poisson random variable](../../../../../poisson-distribution.md) of mean $CT$. In particular,

$$
\mathbb E e^{bN_T}\le\exp\{CT(e^b-1)\}<\infty\qquad(b\ge0).
$$

The case $C=0$ is constant and immediate. For every fixed horizon $T$ and all $s\le T$, including localization times,

$$
0\le M_{s\wedge\tau_n}
\le\exp\{\theta i+\theta_+N_T+(1-e^\theta)_+CT\}.
$$

This is one integrable dominating variable for the entire stopped family. Conditional [dominated convergence](../../../../../dominated-convergence-theorem.md) removes the localization and proves

$$
\boxed{\mathbb E[M_t\mid\mathcal F_s]=M_s\quad(s\le t),}
$$

so the [exponential martingale of a pure birth process](../../../../../exponential-martingale-of-a-pure-birth-process.md) is a genuine [martingale](../../../../../martingale-split.md) for uniformly bounded rates. Only [uniform integrability](../../../../../uniform-integrability.md) on each finite horizon is asserted; it need not be [uniformly integrable](../../../../../uniform-integrability.md) over infinite time.

For a random initial state, the same proof requires $\mathbb E e^{\theta X_0}<\infty$. The source does not explicitly specify the initial distribution, so that qualification cannot be dropped: take constant rate one and an independent initial law $\mathbb P(X_0=n)=6/(\pi^2n^2)$. For $\theta>0$, already $\mathbb EM_0=\infty$, precluding even the integrability in the definition of a [martingale](../../../../../martingale-split.md). The fixed-initial-state interpretation above supplies the intended complete proof; bounded rates alone do not remedy an arbitrary heavy-tailed initial law.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
