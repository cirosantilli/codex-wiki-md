<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Q$ be the given [risk-neutral measure](../../../../../../risk-neutral-measure.md), and write $B_t=B_0e^{rt}$. Take $V$ to be classical on $t<T$ and continuous at its prescribed terminal value. By [Itô formula](../../../../../../ito-s-lemma.md) and the [pricing equation for a local volatility model](../../../../../../pricing-equation-for-a-local-volatility-model.md),

$$
\begin{aligned}
dV(t,S_t)&=\left[V_t+rS_tV_S+\tfrac12\sigma(S_t)^2S_t^2V_{SS}\right]dt+\sigma(S_t)S_tV_S\,d\widehat W_t\\
&=rV(t,S_t)dt+\sigma(S_t)S_tV_S\,d\widehat W_t,
\end{aligned}
$$

so

$$
d\left(\frac{\xi_t}{B_t}\right)=\frac{\sigma(S_t)S_tV_S(t,S_t)}{B_t}\,d\widehat W_t.
$$

The discounted added asset is a [local martingale](../../../../../../local-martingale.md), as is $S_t/B_t$, while $B_t/B_t=1$. Consequently $Q$ is an [equivalent local martingale measure](../../../../../../equivalent-local-martingale-measure.md) for all three assets.

Here is the [arbitrage](../../../../../../arbitrage.md) argument, including the usual [admissible trading strategy](../../../../../../admissible-trading-strategy.md) condition. If $X$ is the discounted wealth of a [self-financing strategy](../../../../../../self-financing-portfolio.md), it is a [stochastic integral](../../../../../../stochastic-integral.md) against the discounted asset prices, plus its initial value, and hence a [local martingale](../../../../../../local-martingale.md). Assume $X_t\geq-c$ for a fixed $c$, as required for an [admissible trading strategy](../../../../../../admissible-trading-strategy.md). For a localizing sequence $\tau_n$, the [stopped process](../../../../../../stopped-process.md) $X^{\tau_n}$ is a [martingale](../../../../../../martingale-split.md). Apply the conditional [Fatou lemma](../../../../../../fatou-s-lemma.md) to $X_{t\wedge\tau_n}+c\geq0$: for $s\leq t$, continuity and the stopped [martingale](../../../../../../martingale-split.md) identity give $\mathbb E_Q[X_t+c\mid\mathcal F_s]\leq X_s+c$. Thus $X$ is a [supermartingale](../../../../../../supermartingale.md). An [arbitrage](../../../../../../arbitrage.md) would have $X_0=0$, $X_T\geq0$ and positive [probability](../../../../../../probability.md) of $X_T>0$. Equivalence of $P,Q$ makes that [probability](../../../../../../probability.md) positive under $Q$, contradicting $\mathbb E_Q[X_T]\leq0$. Therefore **the augmented market has no admissible [arbitrage](../../../../../../arbitrage.md)**.

Nonnegativity of $V$ gives the needed price process, but does not by itself make its discounted [local martingale](../../../../../../local-martingale.md) a true [martingale](../../../../../../martingale-split.md). If $V$ is bounded, the latter follows by bounded [localization](../../../../../../localization-of-a-ring.md), and its price is also $B_t\mathbb E_Q[g(S_T)/B_T\mid\mathcal F_t]$. The [arbitrage](../../../../../../arbitrage.md) proof above applies to the stated nonnegative classical solution without assuming that additional bound.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
