<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $a,b,\mu>0$ and a current state with $0<p<1$, $\beta>0$. The unnormalized [posterior density](../../../../../posterior-density.md) is

$$
\pi(p,\beta\mid x)\ \propto\
\exp\{\ell(p,\beta;x)\}\,p^{a-1}(1-p)^{b-1}\,\mu^{-1}e^{-\beta/\mu}.
$$

Thus the [log-posterior](../../../../../log-posterior.md), up to an additive constant, is the [log-likelihood](../../../../../log-likelihood.md) plus the [beta distribution](../../../../../beta-distribution.md) and [exponential distribution](../../../../../exponential-distribution.md) log [prior densities](../../../../../prior-density.md). The [exponential distribution](../../../../../exponential-distribution.md) rate is $1/\mu$, since $\mu$ is its mean. [Official R documentation: dbeta arguments and logarithmic density output](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/Beta.html) [Official R documentation: dexp rate parameter and mean equal to inverse rate](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/Exponential.html)

Choose a symmetric joint [random-walk Metropolis algorithm](../../../../../random-walk-metropolis-algorithm.md) proposal: $p'=p+0.1G_1$ and $\beta'=\beta+(\mu/2)G_2$, for [independent](../../../../../independent-random-variables.md) [standard normal distribution](../../../../../standard-normal-distribution.md) draws. Its scale depends only on fixed hyperparameters, so forward and reverse proposal [probability density functions](../../../../../probability-density-function.md) agree. Reject immediately outside $(0,1)\times(0,\infty)$; otherwise accept with [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md)

$$
\boxed{\alpha=\min\{1,\exp[\log\pi(p',\beta'\mid x)-\log\pi(p,\beta\mid x)]\}.}
$$

The following function makes exactly one proposal, with rejection retaining both old parameters:

```
MHstep <- function(x, p, beta, a, b, mu) {
  p_new <- rnorm(1, mean = p, sd = 0.1)
  beta_new <- rnorm(1, mean = beta, sd = mu / 2)
  if (p_new <= 0 || p_new >= 1 || beta_new <= 0)
    return(list(p = p, theta = beta))
  logpost <- function(pp, bb) {
    ll_f(pp, bb, x) + dbeta(pp, a, b, log = TRUE) +
      dexp(bb, rate = 1 / mu, log = TRUE)
  }
  logA <- logpost(p_new, beta_new) - logpost(p, beta)
  if (log(runif(1)) <= min(0, logA)) {
    p <- p_new
    beta <- beta_new
  }
  list(p = p, theta = beta)
}
```

**The returned field `theta` contains the updated value of `beta`.** The original PDF really asks for `p` and `theta`, although no parameter $\theta$ is defined in this question. This choice preserves its literal interface while making the intended second parameter explicit. A caller therefore advances with `state <- MHstep(x, p, beta, a, b, mu)`, `p <- state$p`, and `beta <- state$theta`.

The proposal is an unrestricted symmetric [normal distribution](../../../../../normal-distribution.md) followed by rejection outside the [support](../../../../../support.md). Repeatedly drawing until a valid proposal appears would instead truncate and renormalize the proposal, requiring a proposal-density correction. The code uses immediate rejection and needs no such correction. The displayed scales are valid fixed choices; practical efficiency can be improved using a separate tuning phase.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
