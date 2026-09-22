<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

A [uniform prior](../../../../../../uniform-prior.md) on $(0,T)$ makes the [posterior density](../../../../../../posterior-density.md) proportional to the [Poisson change-point posterior](../../../../../../poisson-change-point-posterior.md) likelihood above. The [zeros trick](../../../../../../zeros-trick.md) introduces an observed zero with [Poisson distribution](../../../../../../poisson-distribution.md) mean $K-\log L(\theta)$, making its [likelihood function](../../../../../../likelihood-function.md) equal to $e^{-K}L(\theta)$. Choose $K=T+n\log2+1$; since $\log L(\theta)\le n\log2$, this mean is strictly positive. Rough [BUGS](../../../../../../bugs.md) code, with `zero=0` supplied as data, is
```
model {
  theta ~ dunif(0,T)
  for (i in 1:n) {
    before[i] <- step(theta-time[i])
  }
  j <- sum(before[])
  logL <- theta-2*T+(n-j)*log(2)
  zero ~ dpois(K-logL)
}
```
For $n=0$, omit the array and set `j <- 0`. Monitor the sampled `theta` to obtain its [posterior mean](../../../../../../posterior-mean.md), [credible interval](../../../../../../credible-interval.md) and interval probabilities.

There is also an exact sampling method. On $(t_j,t_{j+1})$ the [posterior density](../../../../../../posterior-density.md) is proportional to $2^{-j}e^\theta$, so choose the interval with weights

$$
w_j=2^{-j}(e^{t_{j+1}}-e^{t_j}),\qquad j=0,\ldots,n.
$$

Then draw $U$ from a [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$ and set $\theta=\log(e^{t_j}+U(e^{t_{j+1}}-e^{t_j}))$. **These weighted interval draws sample the posterior directly**, without asking a local [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) update to cross its discontinuities.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
