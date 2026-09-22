<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Introduce independent component indicators $z_i\mid q\sim\operatorname{Bernoulli}(q)$, and auxiliary slab effects $u_i\sim N(0,V)$, independent of the indicators. Set $\theta_i=z_i u_i$. Then inactive genes have exactly zero effect, while active genes have the stipulated normal distribution. With $V>0$ supplied as known data and elicited positive beta shapes, one suitable [WinBUGS](../../../../../../winbugs.md) model is
```
model {
q ~ dbeta(aq, bq)
for (i in 1:N) {
z[i] ~ dbern(q)
u[i] ~ dnorm(0, 1/V)
theta[i] <- z[i]*u[i]
y[i] ~ dnorm(theta[i], 1)
}
}
```
The normal arguments are precisions, not variances. Supply all observed `y` values, monitor `q`, `theta` and optionally `z`, and assess [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md). The proper auxiliary prior remains defined for inactive genes, where $u_i$ is not informed by the likelihood. This represents the exact [point-null mixture prior](../../../../../../point-null-mixture-prior.md), rather than replacing its point mass by a narrow continuous spike. Conditional on the indicators, $q\mid z$ has [Beta distribution](../../../../../../beta-distribution.md) $\operatorname{Beta}(a_q+\sum_i z_i,b_q+N-\sum_i z_i)$, providing a useful check on the update.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
