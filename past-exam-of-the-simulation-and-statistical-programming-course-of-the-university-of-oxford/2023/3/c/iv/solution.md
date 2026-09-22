<h1 id="3/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose $k$ distinct coordinates uniformly for the starting ones; each element of $S_k$ then has starting [probability](../../../../../probability.md) $1/\binom nk$. At each iteration choose one current one and one current zero uniformly and swap them. This implements the normalized [proposal distribution](../../../../../proposal-distribution.md) from (c)(i), remains in $S_k$, and needs just one precomputed [matrix inverse](../../../../../matrix-inverse-split.md).

```
mymcmc <- function(x, k, sigma) {
  n <- length(x)
  stopifnot(length(k) == 1L, is.finite(k), k == floor(k),
            k > 0L, k < n, is.matrix(sigma),
            all(dim(sigma) == c(n, n)))
  sigma_inv <- invsigma(sigma)
  u <- integer(n)
  u[sample.int(n, k, replace = FALSE)] <- 1L
  draws <- matrix(0, 100L, n)
  for (iteration in seq_len(100L)) {
    ones <- which(u == 1L)
    zeros <- which(u == 0L)
    i <- ones[sample.int(length(ones), 1L)]
    j <- zeros[sample.int(length(zeros), 1L)]
    v <- u
    v[i] <- 0L
    v[j] <- 1L
    alpha <- mylogapp(x, u, v, sigma_inv)
    if (runif(1L) < alpha) u <- v
    draws[iteration, ] <- u
  }
  colMeans(draws)
}
```

Sampling positions with `sample.int` and then indexing into `ones` or `zeros` also works when $k=1$ or $n-k=1$. In [R](../../../../../r-programming-language.md), a call such as `sample(ones, 1)` would incorrectly sample from `1:ones` when `ones` is a single numeric value greater than one.

The code records the state after each of exactly $100$ transitions, including repetitions after rejection. Its answer is the vector [Monte Carlo estimator](../../../../../monte-carlo-estimator.md)

$$
\boxed{\widehat m=\frac1{100}\sum_{t=1}^{100}U^{(t)}\approx\mathbb E[U\mid X=x].}
$$

This estimates the [posterior mean](../../../../../posterior-mean.md) coordinate by coordinate; because each coordinate is binary, its entries estimate the [posterior probabilities](../../../../../posterior-probability.md) of inclusion. Every stored state has coordinate sum $k$, so the estimated means lie in $[0,1]$ and sum to $k$.

For neighbouring states, the symmetry of the proposal and the [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md) give [detailed balance](../../../../../detailed-balance.md):

$$
\pi(u\mid x)q(v\mid u)\alpha(u,v)
=q(v\mid u)\min\{\pi(u\mid x),\pi(v\mid x)\}
=\pi(v\mid x)q(u\mid v)\alpha(v,u).
$$

Thus the [posterior distribution](../../../../../bayesian-posterior.md) is a [stationary distribution](../../../../../stationary-distribution.md). Any two states in $S_k$ can be connected by moving the ones that occupy the wrong positions, and the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) gives strictly positive target masses. The resulting [Markov chain](../../../../../markov-chain-split.md) is therefore an [irreducible Markov chain](../../../../../irreducible-markov-chain.md), and its long-run state averages estimate the [posterior mean](../../../../../posterior-mean.md).

The requested $100$ iterations are a finite approximation, without a convergence guarantee or discarded [burn-in](../../../../../burn-in.md). A randomly chosen starting subset has the [prior distribution](../../../../../prior-probability.md), rather than generally the [posterior distribution](../../../../../bayesian-posterior.md). No [aperiodicity](../../../../../aperiodic-markov-chain.md) assumption is needed for the finite-state [Markov chain ergodic theorem](../../../../../markov-chain-ergodic-theorem.md) for averages; indeed a uniform two-state target with $n=2,k=1$ gives a period-two alternating chain. This does not invalidate either the code or the state-average estimator.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
