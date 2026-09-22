<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat each observed arrival label as a constraint on an unobserved walking duration. Departures are treated as fixed design information. Writing $c$ for the minutes available until work starts, the derived late-label thresholds have frequencies $20:1,21:3,25:3,27:1,32:2$; the early-label thresholds have frequencies $29:1,34:1,36:3,37:1,38:1,39:1,43:1,44:1$. These are [censoring](../../../../../censoring-statistics.md) thresholds, **not measured journey times**. A late label means $T>c$, and an early label means $T<c$; equality has [probability](../../../../../probability.md) zero under the continuous model.

The paper specifies no [prior distribution](../../../../../prior-probability.md). One explicit proper model is

$$
\mu\sim\operatorname{Unif}(0,60),\qquad \sigma\sim\operatorname{Unif}(1,20),\qquad T_i\mid\mu,\sigma\overset{\rm iid}{\sim}N(\mu,\sigma^2),
$$

with independent priors; all times are in minutes. These ranges are a transparent modelling choice, not information deduced from the observations. In particular, this is a prior on the [standard deviation](../../../../../standard-deviation.md) $\sigma$, not a uniform prior on the [variance](../../../../../variance-split.md) $\sigma^2$. The [normal distribution](../../../../../normal-distribution.md) permits negative durations; it is the mathematical approximation requested here, rather than a claim that such durations are physically possible. A truncated model would be a different model.

The following [Python](../../../../../python-programming-language.md) implements hard conditioning by [rejection sampling](../../../../../rejection-sampling.md). `None` marks a rejected trace; an accepted [Boolean](../../../../../boolean-data-type.md) answers whether all five future arrivals are late. The same parameters are shared across past and future days.

```
import math
import random

LATE = {20: 1, 21: 3, 25: 3, 27: 1, 32: 2}
EARLY = {29: 1, 34: 1, 36: 3, 37: 1, 38: 1, 39: 1, 43: 1, 44: 1}
RECORDS = [(c, True) for c, n in LATE.items() for _ in range(n)]
RECORDS += [(c, False) for c, n in EARLY.items() for _ in range(n)]

def journey_trace(rng):
    mu = rng.uniform(0.0, 60.0)
    sigma = rng.uniform(1.0, 20.0)
    # Twenty latent past durations and five future durations.
    past = [rng.gauss(mu, sigma) for _ in RECORDS]
    future = [rng.gauss(mu, sigma) for _ in range(5)]
    if not all(t > c if late else t < c
               for t, (c, late) in zip(past, RECORDS)):
        return None
    return all(t > 30.0 for t in future)

def accepted_average(trace, n, rng):
    if n <= 0:
        raise ValueError("n must be positive")
    successes = accepted = 0
    while accepted < n:
        result = trace(rng)
        if result is not None:
            accepted += 1
            successes += int(result)
    return successes / n
```

For example, `accepted_average(journey_trace, n, random.Random(2021))` estimates the desired [conditional probability](../../../../../conditional-probability.md) from $n$ accepted traces. Accepting `False` is essential: treating a false answer as a rejected trace would condition on the desired conclusion. The model deliberately emphasizes clear semantics; rejection can be inefficient because all twenty past-label constraints must hold together.

## ↑ Ancestors (11)

1. [A](../a.md)
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
