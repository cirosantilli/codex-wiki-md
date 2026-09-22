<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider a [binomial market](../../../../../../discrete-time-binomial-market.md) with dates $0,\ldots,n$, bank account $B_k=b^k$ for $b>0$, and [stock](../../../../../../stock.md) price $S_{k+1}=S_ku$ or $S_kd$, where $0<d<u$. Both moves have positive physical probability, and the information at date $k$ is the history of the first $k$ moves. Absence of [arbitrage](../../../../../../arbitrage.md) requires and is implied by $d<b<u$. If $b\leq d$, borrowing cash to buy [stock](../../../../../../stock.md) has nonnegative payoff with a strict gain in one state; if $b\geq u$, the reverse trade does. In the interior range, the [risk-neutral probability](../../../../../../risk-neutral-probability.md) of an up move is

$$
\boxed{q=\frac{b-d}{u-d}\in(0,1).}
$$

It makes $\mathbb E_Q[S_{k+1}\mid\mathcal F_k]=bS_k$, so $S_k/B_k$ is a [martingale](../../../../../../martingale-split.md). This proves absence of arbitrage by pricing discounted gains under the equivalent measure.

At a node with [stock](../../../../../../stock.md) price $s$, let the desired next-period [portfolio](../../../../../../investment-portfolio.md) values be $V_u,V_d$. Solve the two replication equations $\Delta su+\beta B_{k+1}=V_u$ and $\Delta sd+\beta B_{k+1}=V_d$. The [replicating portfolio in a binomial market](../../../../../../replicating-portfolio-in-a-binomial-market.md) has

$$
\boxed{\Delta_k=\frac{V_u-V_d}{s(u-d)},\qquad\beta_kB_k=\frac{uV_d-dV_u}{b(u-d)}.}
$$

Its current value is

$$
\boxed{V_k=\Delta_ks+\beta_kB_k=\frac{qV_u+(1-q)V_d}{b}.}
$$

Rebalance at the next node using exactly the value supplied by the previous holdings, so the strategy is [self-financing](../../../../../../self-financing-portfolio.md). Backward induction from any terminal [contingent claim](../../../../../../contingent-claim.md) $H$ gives its hedge and the unique price

$$
V_k=B_k\mathbb E_Q[H/B_n\mid\mathcal F_k].
$$

Thus the finite binomial market is a [complete market](../../../../../../complete-market.md). The construction works for path-dependent claims on the full history tree, even when their values do not recombine merely as functions of the current [stock](../../../../../../stock.md) price. For $H=f(S_n)$, independence under $Q$ gives the explicit time-zero price

$$
\boxed{V_0=b^{-n}\sum_{j=0}^n\binom njq^j(1-q)^{n-j}f(S_0u^jd^{n-j}).}
$$

The [stock](../../../../../../stock.md) hedge is a difference quotient of successor values, the discrete analogue of the [delta hedge](../../../../../../delta-hedge.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
