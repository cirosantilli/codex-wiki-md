<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Represent the independent locally flat intercept [prior distributions](../../../../../../prior-probability.md) by broad finite [uniform priors](../../../../../../uniform-prior.md), for example on $(-10,10)$; this is proper and approximately constant over plausible mortality logits. With $A$ calibrated above, rough [BUGS](../../../../../../bugs.md) code is
```
model {
  mu ~ dnorm(0,0.25)
  tau ~ dunif(0,A)
  invtau2 <- pow(tau,-2)
  for (j in 1:J) {
    alpha[j] ~ dunif(-10,10)
    beta[j] ~ dnorm(mu,invtau2)
    logit(thetaC[j]) <- alpha[j]-beta[j]/2
    logit(thetaT[j]) <- alpha[j]+beta[j]/2
    rC[j] ~ dbin(thetaC[j],nC[j])
    rT[j] ~ dbin(thetaT[j],nT[j])
    oddsRatio[j] <- exp(beta[j])
  }
}
```
Use $J=6$ and supply treated death counts $(3,7,5,102,32,22)$ with totals $(38,114,69,1533,209,680)$, and control death counts $(3,14,11,127,40,39)$ with totals $(39,116,93,1520,218,674)$. In [BUGS](../../../../../../bugs.md), the second `dnorm` argument is a [precision parameter](../../../../../../precision-parameter.md), so `0.25` corresponds to [variance](../../../../../../variance-split.md) four. Initialize the positive scale away from zero. Monitor $\mu,\tau$ and study [odds ratios](../../../../../../odds-ratio.md), checking [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md) and sensitivity to the finite intercept bounds and scale [prior distribution](../../../../../../prior-probability.md). **The fitted hierarchy combines binomial sampling uncertainty with between-study heterogeneity.**

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
