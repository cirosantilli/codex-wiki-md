<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n$ observed complete independent exponential gaps, let $T_n=\sum_{i=1}^n\tau_i$. The [likelihood function](../../../../../../likelihood-function.md) is $L(\lambda)=\lambda^ne^{-\lambda T_n}$, and the [log-likelihood](../../../../../../log-likelihood.md) has derivative $n/\lambda-T_n$ and second derivative $-n/\lambda^2<0$. Hence the unique [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\lambda=n/T_n=1/\overline\tau.}
$$

Alternatively, observe $m$ unit-year increments $Y_j=N_j-N_{j-1}$. These are independent Poisson counts of [mean](../../../../../../expected-value.md) $\lambda$. Their joint likelihood is proportional to $\lambda^{\sum Y_j}e^{-m\lambda}$, giving

$$
\boxed{\widehat\lambda=\frac1m\sum_{j=1}^mY_j=N_m/m.}
$$

It is unbiased, with [variance](../../../../../../variance-split.md) $\lambda/m$. A zero observed count gives the boundary estimate zero, or the supremum as $\lambda\downarrow0$ if the parameter space is restricted to positive rates.

The [Poisson observation scheme and rate likelihood](../../../../../../poisson-observation-scheme-and-rate-likelihood.md) distinction matters when comparing the techniques. For a fixed observation horizon, conditional on the total number of events the event locations have a distribution independent of $\lambda$. Thus exact timestamps add no rate information to the total count under the homogeneous Poisson model; unit-interval counts already contain that total. The correct fixed-horizon likelihood includes the final unfinished waiting interval, and gives count divided by the full exposure, not by the sum of only completed gaps.

The first calculation instead stops after a fixed number $n$ of events, so its exposure $T_n$ is random. Its estimate has [mean](../../../../../../expected-value.md) $n\lambda/(n-1)$ for $n>1$ and an infinite [mean](../../../../../../expected-value.md) for $n=1$, unlike the unbiased fixed-horizon count estimate. For $n>2$ its [variance](../../../../../../variance-split.md) is $n^2\lambda^2/[(n-1)^2(n-2)]$, asymptotic to $\lambda^2/n$. There is no universally more informative sampling technique without specifying the stopping rule and exposure. Counts are sufficient and convenient for estimating a truly constant rate; timestamps additionally help diagnose departures from constant intensity or independent gaps.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
