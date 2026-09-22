<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [delta replication from a local-volatility pricing equation](../../../../../../delta-replication-from-a-local-volatility-pricing-equation.md) uses the asset-unit holdings

$$
\boxed{h^S_t=V_S(t,S_t),\qquad h^B_t=\frac{V(t,S_t)-S_tV_S(t,S_t)}{B_t}.}
$$

Their wealth is exactly $V(t,S_t)$. Moreover,

$$
h^B_t\,dB_t+h^S_t\,dS_t=rV(t,S_t)dt+\sigma(S_t)S_tV_S(t,S_t)d\widehat W_t=dV(t,S_t),
$$

where the final equality is the calculation in part (i). Thus the holdings are a [self-financing strategy](../../../../../../self-financing-portfolio.md) with terminal wealth $g(S_T)$, proving replication. Since $V\geq0$, this [replicating strategy](../../../../../../replicating-strategy.md) has nonnegative wealth and is an [admissible trading strategy](../../../../../../admissible-trading-strategy.md). The equality of trading gains is unchanged by replacing the drift with its physical-measure value: the stock drift in [Itô formula](../../../../../../ito-s-lemma.md) and in the stock holding changes by the same amount. If $\pi_t$ denotes wealth fractions, then, wherever $V>0$, its stock fraction is $S_tV_S/V$ and its bank fraction is $1-S_tV_S/V$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
