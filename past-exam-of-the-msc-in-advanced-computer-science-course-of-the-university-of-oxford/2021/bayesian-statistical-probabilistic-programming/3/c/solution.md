<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\Phi$ for the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). Integrating out the twenty independent past durations gives the [threshold-censored normal likelihood](../../../../../threshold-censored-normal-likelihood.md)

$$
L(\mu,\sigma)=\prod_{c\in C_L}\Phi\left(\frac{\mu-c}{\sigma}\right)^{n_L(c)}\prod_{c\in C_E}\Phi\left(\frac{c-\mu}{\sigma}\right)^{n_E(c)}.
$$

The frequencies $n_L,n_E$ are those in part (a). For a future day, the conditional late-arrival [probability](../../../../../probability.md) is $\pi(\mu,\sigma)=\Phi((\mu-30)/\sigma)$. [Conditional independence](../../../../../conditional-independence.md) of the five future durations gives $h(\mu,\sigma)=\pi(\mu,\sigma)^5$.

Exactly three primitive random coordinates suffice. Draw $\mu,\sigma$ from the same priors and one independent $U\sim\operatorname{Unif}(0,1)$. Reject if $U\geq L(\mu,\sigma)$; otherwise return whether $U<L(\mu,\sigma)h(\mu,\sigma)$. Conditional on acceptance and the parameters, $U$ is uniform on an interval of length $L$; the true-answer subinterval has length $Lh$. Reusing this same uniform value is therefore intentional, not an independence mistake.

Indeed the two output contributions at each parameter value are

$$
\mathbb P(A,Y=1\mid\mu,\sigma)=Lh,\qquad \mathbb P(A,Y=0\mid\mu,\sigma)=L(1-h).
$$

These are exactly the contributions obtained by integrating the original twenty-five duration noises. Multiplication by the common [prior density](../../../../../prior-density.md) and [normalization](../../../../../normalization.md) therefore give the same joint [posterior distribution](../../../../../bayesian-posterior.md) of $(\mu,\sigma,Y)$. The revised program preserves the query and parameter posterior, but does not retain individual latent durations. This is [uniform-interval encoding of conditioning and a binary query](../../../../../uniform-interval-encoding-of-conditioning-and-a-binary-query.md).

Here is an executable version, reusing the definitions from part (a). [Logarithms](../../../../../logarithm.md) avoid multiplying many small [probabilities](../../../../../probability.md).

```
def normal_logcdf(z):
    value = 0.5 * math.erfc(-z / math.sqrt(2.0))
    return math.log(value) if value > 0.0 else -math.inf

def journey_loglik(mu, sigma):
    return (sum(n * normal_logcdf((mu - c) / sigma)
                for c, n in LATE.items())
            + sum(n * normal_logcdf((c - mu) / sigma)
                  for c, n in EARLY.items()))

def collapsed_trace(rng):
    mu = rng.uniform(0.0, 60.0)
    sigma = rng.uniform(1.0, 20.0)
    log_likelihood = journey_loglik(mu, sigma)
    # This uniform lies in (0, 1], avoiding log(0).
    log_u = math.log(1.0 - rng.random())
    if log_u >= log_likelihood:
        return None
    log_h = 5.0 * normal_logcdf((mu - 30.0) / sigma)
    return log_u < log_likelihood + log_h
```

`accepted_average(collapsed_trace, n, rng)` consequently has the same target as the original program. The ideal three-dimensional [sample space](../../../../../sample-space.md) is $(0,60)\times(1,20)\times(0,1)$ with product uniform [probability measure](../../../../../probability-measure.md), conditioned on the displayed acceptance event. Finite-precision normal tails can underflow to zero in this simple implementation; the mathematical equivalence concerns exact [probabilities](../../../../../probability.md), and the numerical check in part (d) independently integrates the [likelihood](../../../../../likelihood-function.md) in the region carrying appreciable posterior mass.

## ↑ Ancestors (11)

1. [C](../c.md)
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
