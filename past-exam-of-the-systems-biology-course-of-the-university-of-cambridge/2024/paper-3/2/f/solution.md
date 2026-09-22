<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**TODO: Complete the data-specific numerical results and diagnostics when the original `Iris_data.csv` is available.**

Estimate the [posterior mean](../../../../../posterior-mean.md) by averaging the retained states:

$$
\boxed{\widehat{\mathbb E[\mu\mid x]}=\frac1{9000}\sum_{t=1001}^{10000}\mu_t}.
$$

The exact [truncated normal distribution](../../../../../truncated-normal-distribution.md) reference is

$$
\boxed{\mathbb E[\mu\mid x]=m+s\frac{\phi(m/s)}{\Phi(m/s)}},\qquad
m=\bar x-\frac1{3n},\quad s=n^{-1/2}.
$$

For a [posterior](../../../../../bayesian-posterior.md) well separated from zero, the truncation correction is tiny and the [posterior mean](../../../../../posterior-mean.md) is approximately $\bar x-1/(3n)$, slightly below the [sample mean](../../../../../sample-mean.md).

The R continuation prints the [Monte Carlo estimator](../../../../../monte-carlo-estimator.md), its approximate batch-based [Monte Carlo standard error](../../../../../monte-carlo-standard-error.md), and the exact value for comparison:

```
posterior_mean_mc <- mean(post)
posterior_mean_exact <- m + s * exp(dnorm(m/s, log = TRUE) -
                                    pnorm(m/s, log.p = TRUE))
# Nonoverlapping batches account approximately for serial dependence.
batch_length <- floor(sqrt(length(post)))
number_batches <- floor(length(post)/batch_length)
used <- post[seq_len(batch_length * number_batches)]
batch_averages <- colMeans(matrix(used, nrow = batch_length))
mcse <- sd(batch_averages)/sqrt(number_batches)
cat("Posterior mean, MCMC =", posterior_mean_mc,
    " approximate MCSE =", mcse, "\n")
cat("Posterior mean, exact =", posterior_mean_exact, "\n")
```

The batch length must be long enough relative to the chain's dependence for this uncertainty estimate to be reliable. **No numerical data-specific [posterior mean](../../../../../posterior-mean.md) is determined by the supplied paper alone.**

## ↑ Ancestors (13)

1. [F](../f.md)
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
