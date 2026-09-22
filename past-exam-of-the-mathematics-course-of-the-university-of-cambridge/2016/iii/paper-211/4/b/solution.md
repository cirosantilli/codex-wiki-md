<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the usual no-[arbitrage](../../../../../../arbitrage.md) interpretation from part (a), let $Q^N$ be an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) for the strictly positive [numéraire](../../../../../../numeraire.md) $N$. Then $M_t=S_t/N_t$ is a [martingale](../../../../../../martingale-split.md). Define the discounted [European call option](../../../../../../european-call-option.md) payoff $Y_t=(S_t-K)^+/N_t=(M_t-K/N_t)^+$. Because $N_{t+1}\geq N_t$ and $K>0$, we have $K/N_{t+1}\leq K/N_t$. The [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md) therefore gives

$$
\begin{aligned}
\mathbb E^{Q^N}[Y_{t+1}\mid\mathcal F_t]
&\geq\mathbb E^{Q^N}[(M_{t+1}-K/N_t)^+\mid\mathcal F_t]\\
&\geq\big(\mathbb E^{Q^N}[M_{t+1}\mid\mathcal F_t]-K/N_t\big)^+
=Y_t.
\end{aligned}
$$

For the middle step, the strike $K/N_t$ is fixed conditionally on $\mathcal F_t$; alternatively use $\mathbb E[X^+\mid\mathcal F_t]\geq\max\{\mathbb E[X\mid\mathcal F_t],0\}$. Thus $Y$ is a [submartingale](../../../../../../submartingale.md). [Risk-neutral valuation](../../../../../../risk-neutral-pricing.md) in units of $N$ gives $C(T,K)=N_0\mathbb E^{Q^N}Y_T$, with the usual fixed initial prices. **Consequently**

$$
\boxed{C(T+1,K)\geq C(T,K).}
$$

The source's word “increasing” means nondecreasing: a [European call option](../../../../../../european-call-option.md) can have zero payoff at successive maturities, so strict increase is not guaranteed. Integrability is understood in the claim class for which the stated replication prices exist.

## ↑ Ancestors (11)

1. [B](../b.md)
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
