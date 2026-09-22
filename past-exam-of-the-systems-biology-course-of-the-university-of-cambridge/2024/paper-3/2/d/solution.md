<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**TODO: Complete the data-specific numerical results and diagnostics when the original `Iris_data.csv` is available.**

Use the [random-walk Metropolis algorithm](../../../../../random-walk-metropolis-algorithm.md) with proposal $\mu'=\mu+\varepsilon$, where $\varepsilon\sim N(0,1)$. The proposal is symmetric, so for a nonnegative proposal the acceptance [probability](../../../../../probability.md) is

$$
\boxed{a(\mu,\mu')=\min\{1,\exp[\ell_p(\mu')-\ell_p(\mu)]\}},\qquad
\ell_p(u)=-\frac12\sum_i(x_i-u)^2-\frac u3.
$$

Negative proposals are rejected. They are not redrawn until positive, since that would change the proposal kernel and require a different acceptance ratio. On rejection, store the current state again; keeping accepted moves alone would bias the empirical [posterior distribution](../../../../../bayesian-posterior.md).

This R continuation makes exactly 10,000 proposals, starting at $\mu_0=4$:

```
set.seed(20240528)
B <- 10000L
mu <- numeric(B + 1L)
mu[1L] <- 4
logpost <- function(u) {
  if (!is.finite(u) || u < 0) return(-Inf)
  loglik(u) - u/3
}
lp <- logpost(mu[1L])
accepted <- 0L
for (i in seq_len(B)) {
  proposal <- rnorm(1L, mean = mu[i], sd = 1)
  lp_new <- logpost(proposal)
  if (log(runif(1L)) < min(0, lp_new - lp)) {
    mu[i + 1L] <- proposal
    lp <- lp_new
    accepted <- accepted + 1L
  } else {
    mu[i + 1L] <- mu[i]
  }
}
cat("Acceptance fraction =", accepted/B, "\n")
# A provisional discard; assess it with the trace in part (e).
burn <- 1000L
post <- mu[(burn + 2L):(B + 1L)]
m <- xbar - 1/(3*n)
s <- 1/sqrt(n)
posterior_density <- function(u) {
  ans <- numeric(length(u))
  ok <- u >= 0
  ans[ok] <- exp(dnorm(u[ok], m, s, log = TRUE) -
                   pnorm(m/s, log.p = TRUE))
  ans
}
png("q2-posterior.png", width = 900, height = 600)
hist(post, breaks = 40, probability = TRUE, xlab = expression(mu),
     main = "Retained Metropolis draws and exact posterior")
u <- seq(0, max(post) + 3*s, length.out = 4001L)
lines(u, posterior_density(u), col = "firebrick", lwd = 2)
dev.off()
```

The exact [truncated normal distribution](../../../../../truncated-normal-distribution.md) density overlays the histogram as a check; it does not replace the requested [Markov chain Monte Carlo](../../../../../markov-chain-monte-carlo.md) procedure. The 9,000 retained states exclude the initial state and the first 1,000 transitions. The particular histogram and acceptance fraction remain dependent on the missing measurements.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
