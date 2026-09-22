<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

I would first collapse the duration noises as in part (c), then use [self-normalized importance sampling](../../../../../self-normalized-importance-sampling.md) on the two shared parameters. Draw independent $(\mu_j,\sigma_j)\sim\rho$, give each the [importance weight](../../../../../importance-weight.md) $w_j=L(\mu_j,\sigma_j)$, and return

$$
\boxed{\widehat P_N=\frac{\sum_{j=1}^Nw_j\pi(\mu_j,\sigma_j)^5}{\sum_{j=1}^Nw_j}.}
$$

This is [likelihood weighting](../../../../../likelihood-weighting.md): the observations affect the weights rather than forcing repeated simulation of twenty latent inequalities. Integrating out both the constraints' auxiliary randomness and the future [Boolean](../../../../../boolean-data-type.md) query is [Rao-Blackwellization](../../../../../rao-blackwellization.md); at fixed parameters it removes randomness without changing the relevant [conditional expectations](../../../../../conditional-expectation.md).

The weights and weighted queries lie in $[0,1]$, and the evidence is positive. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) therefore makes the numerator and denominator averages converge to their corresponding integrals, proving [almost sure convergence](../../../../../almost-sure-convergence.md) of their ratio to part (d). The finite-$N$ ratio is generally biased; the assertion concerns consistency rather than a finite-sample [unbiased estimator](../../../../../unbiased-estimator.md). Use [logarithms](../../../../../logarithm.md) of [importance weights](../../../../../importance-weight.md) to avoid numerical underflow:

```
def weighted_answer(n, rng):
    if n <= 0:
        raise ValueError("n must be positive")
    samples = []
    for _ in range(n):
        mu = rng.uniform(0.0, 60.0)
        sigma = rng.uniform(1.0, 20.0)
        samples.append((journey_loglik(mu, sigma),
                        math.exp(5.0 * normal_logcdf((mu - 30.0) / sigma))))
    offset = max(logw for logw, h in samples)
    if not math.isfinite(offset):
        raise ArithmeticError("all weights underflowed")
    scaled = [(math.exp(logw - offset), h) for logw, h in samples]
    den = math.fsum(w for w, h in scaled)
    answer = math.fsum(w * h for w, h in scaled) / den
    ess = den * den / math.fsum(w * w for w, h in scaled)
    return answer, ess
```

The returned [effective sample size of importance sampling](../../../../../effective-sample-size-of-importance-sampling.md) is a concentration diagnostic, not a proof of accuracy. Repeat runs and inspect the weights. If the prior is much broader than the posterior, improve the proposal with the corresponding [importance sampling](../../../../../importance-sampling.md) density correction, or use the [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) targeting $\rho L$. Because this particular collapsed problem is only two-dimensional, deterministic [numerical integration](../../../../../numerical-integration-split.md) is also an excellent independent accuracy check; it was used for the figure and numerical illustration. Straight rejection of the original traces is correct but wastes most proposals here.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
