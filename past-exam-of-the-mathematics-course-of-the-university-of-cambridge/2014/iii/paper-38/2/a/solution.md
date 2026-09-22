<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A trading strategy chooses a vector $H_t$ of holdings for the period $(t-1,t]$, with $H_t$ measurable with respect to $\mathcal F_{t-1}$. Its end-of-period wealth is $X_t=H_t\cdot P_t$. Rebalancing at date $t$ is [self-financing](../../../../../../self-financing-portfolio.md) when

$$
H_{t+1}\cdot P_t=H_t\cdot P_t;
$$

new holdings cost exactly the value released by the old holdings. With fixed initial capital $x$, the equivalent gains identity is

$$
\boxed{X_t=x+\sum_{u=1}^t H_u\cdot(P_u-P_{u-1}).}
$$

A [European contingent claim](../../../../../../european-contingent-claim.md) is a maturity-$T$ payoff $\xi$ measurable with respect to $\mathcal F_T$. It is attainable if there exists a [predictable](../../../../../../predictable-process.md) [self-financing strategy](../../../../../../self-financing-portfolio.md) and an initial capital $x$ for which $X_T=\xi$ almost surely. Such a strategy is a [replicating strategy](../../../../../../replicating-strategy.md), and $x$ is its initial replication cost. Holdings are understood only up to the maturity being replicated.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
