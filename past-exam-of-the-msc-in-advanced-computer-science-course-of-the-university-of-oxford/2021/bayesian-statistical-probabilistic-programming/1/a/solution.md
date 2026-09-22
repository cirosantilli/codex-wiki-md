<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $0<Z=\sum_xr(x)<\infty$, and work on the [support](../../../../../support.md) $S=\{x:r(x)>0\}$. In [rejection sampling](../../../../../rejection-sampling.md), choose a normalized proposal [probability mass function](../../../../../probability-mass-function.md) $g$ and a known finite constant $M$ satisfying $r(x)\leq Mg(x)$ everywhere. Draw [independent random variables](../../../../../independent-random-variables.md) $Y\sim g$ and $U\sim\operatorname{Unif}(0,1)$, accepting $Y$ when $U\leq r(Y)/(Mg(Y))$. The joint [probability](../../../../../probability.md) of proposing and accepting $x$ is $r(x)/M$, so the overall acceptance [probability](../../../../../probability.md) is $Z/M$ and the accepted value has [probability mass function](../../../../../probability-mass-function.md) $r(x)/Z$. Fresh trials therefore produce [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with the desired [probability distribution](../../../../../probability-distribution-split.md). For a fixed positive number $N$ of accepted values, the sample average $N^{-1}\sum_{i=1}^Nf(Y_i)$ is an [unbiased estimator](../../../../../unbiased-estimator.md) of the [expectation](../../../../../expected-value-split.md) when that [expectation](../../../../../expected-value-split.md) is finite. Its [variance](../../../../../variance-split.md) is $\operatorname{Var}_p(f)/N$ if the second moment is finite. Finding a valid envelope can be difficult, and a small acceptance [probability](../../../../../probability.md) makes the method expensive.

For the [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md), choose a proposal [transition matrix](../../../../../stochastic-matrix.md) $q$ and, at the current state $x$, propose $y\sim q(x,\cdot)$. Accept with the [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md)

$$
\alpha(x,y)=\min\left\{1,\frac{r(y)q(y,x)}{r(x)q(x,y)}\right\}.
$$

A proposal outside $S$ is rejected; an impossible proposal need not be assigned a ratio. Otherwise remain at $x$. This constructs a [Markov chain](../../../../../markov-chain-split.md) satisfying [detailed balance](../../../../../detailed-balance.md) with $p$, without computing $Z$ or a global envelope. Estimate the [expectation](../../../../../expected-value-split.md) by averaging $f(X_i)$ over iterations, **including repeated states after rejections**. Keeping only accepted jumps generally changes the [stationary distribution](../../../../../stationary-distribution.md) of the recorded process.

The [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) produces dependent samples, so the [variance](../../../../../variance-split.md) of its average includes [autocovariances](../../../../../autocovariance.md); starting outside [stationarity](../../../../../stationary-process.md) can also cause finite-run [bias](../../../../../bias-of-an-estimator.md). With [Markov chain irreducibility](../../../../../irreducible-markov-chain.md), suitable recurrence and an integrable $f$, the [countable-state Markov chain ergodic theorem](../../../../../countable-state-markov-chain-ergodic-theorem.md) gives consistency. [Aperiodicity](../../../../../aperiodic-markov-chain.md) is additionally needed for the usual convergence of one-time [probability distributions](../../../../../probability-distribution-split.md). In contrast, accepted [rejection sampling](../../../../../rejection-sampling.md) values need no initial transient. Neither method is universally faster: envelope rejection competes with the proposal quality and [mixing time](../../../../../mixing-time-of-a-markov-chain.md) of the [Markov chain](../../../../../markov-chain-split.md). Nonnegativity of $f$ alone does not guarantee a finite [expectation](../../../../../expected-value-split.md) or [variance](../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
