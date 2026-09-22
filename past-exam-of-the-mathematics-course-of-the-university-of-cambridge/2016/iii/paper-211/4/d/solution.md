<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The positive-part function is [convex](../../../../../../convex-function.md), so pathwise [Jensen inequality](../../../../../../jensen-s-inequality.md) gives

$$
\left(\frac1T\sum_{t=1}^T S_t-K\right)^+
\leq\frac1T\sum_{t=1}^T(S_t-K)^+.
$$

To compare the [Asian option](../../../../../../asian-option.md) price with [European call option](../../../../../../european-call-option.md) prices at different dates, carry each earlier payoff forward using the [numéraire](../../../../../../numeraire.md). Purchase $1/T$ of each [replicating strategy](../../../../../../replicating-strategy.md) for maturity $t$, and, when its payoff is received, reinvest it in $N$ until $T$. This is a [self-financing portfolio](../../../../../../self-financing-portfolio.md), with terminal wealth

$$
\frac1T\sum_{t=1}^T (S_t-K)^+\frac{N_T}{N_t}
\geq\frac1T\sum_{t=1}^T(S_t-K)^+
\geq\left(\frac1T\sum_{t=1}^T S_t-K\right)^+.
$$

The first inequality uses $N_T\geq N_t$ and nonnegative payoffs. Since the [Asian option](../../../../../../asian-option.md) is replicable in the [complete market](../../../../../../complete-market.md), absence of [arbitrage](../../../../../../arbitrage.md) makes its replication cost no larger than this [superhedging](../../../../../../superhedging.md) cost. **Therefore**

$$
\boxed{A(T,K)\leq\frac1T\sum_{t=1}^T C(t,K).}
$$

Equivalently, divide the first pathwise bound by $N_T$, use $(S_t-K)^+/N_T\leq(S_t-K)^+/N_t$, and take [expectations](../../../../../../expected-value.md) under the [numéraire](../../../../../../numeraire.md) [equivalent martingale measure](../../../../../../risk-neutral-measure.md). Merely averaging earlier payoffs without reinvestment would miss the difference in payment dates.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
