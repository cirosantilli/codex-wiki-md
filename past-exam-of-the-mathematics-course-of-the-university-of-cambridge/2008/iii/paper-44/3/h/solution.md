<h1 id="3/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Add the new individual's latent mean and log variance to the same population hierarchy. Enter only that individual's first two measurements as observations; use the historical data and these two values to fit the model. The third measurement must be held out, or the predictive check reuses the value it is meant to test. For example, augment the unchanged population hyperpriors with this [WinBUGS](../../../../../../winbugs.md) structure:

```
new.mean ~ dnorm(mu, invtau2)
new.logvar ~ dnorm(phi, invpsi2)
new.precision <- exp(-new.logvar)
for (k in 1:2) {
    new.Y[k] ~ dnorm(new.mean, new.precision)
}
future.Y ~ dnorm(new.mean, new.precision)
upper.indicator <- step(future.Y - held.out.third)
```

`future.Y` is unobserved. Its simulated values give the [posterior predictive distribution](../../../../../../posterior-predictive-distribution.md), including uncertainty in the population parameters and personal variance. A central 99.9% [prediction interval](../../../../../../prediction-interval.md) uses its $0.0005$ and $0.9995$ empirical quantiles. **Flag the third value if it is outside that interval.** Equivalently, estimate its predictive tail probability by the mean of `upper.indicator` and flag if that mean is below $0.0005$ or above $0.9995$. This is two-sided, unlike the earlier one-sided upper limit.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
