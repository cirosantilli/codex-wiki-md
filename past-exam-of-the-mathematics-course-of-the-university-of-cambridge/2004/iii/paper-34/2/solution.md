<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let the [bank account](../../../../../bank-account.md) be $B_r=R^r$, where $R>0$ is the one-period riskless gross return. In the [binomial market](../../../../../discrete-time-binomial-market.md), $S_{r+1}$ is either $uS_r$ or $dS_r$, with $0<d<1<u$ and both successors having positive physical [probability](../../../../../probability.md). The information at time $r$ consists of the first $r$ moves. A trading strategy chooses its holdings using only this information. A [self-financing portfolio](../../../../../self-financing-portfolio.md) funds rebalancing from its current value; there is no external contribution.

Absence of [arbitrage](../../../../../arbitrage.md) requires $d<R<u$. If $R\leq d$, borrowing to buy the [stock](../../../../../stock.md) yields a nonnegative gain, strictly positive on the up branch; if $R\geq u$, shorting the [stock](../../../../../stock.md) and investing its price yields the reverse [arbitrage](../../../../../arbitrage.md). When $d<R<u$, define the [risk-neutral probability in a binomial market](../../../../../risk-neutral-probability-in-a-binomial-market.md)

$$
q=\frac{R-d}{u-d}\in(0,1),\qquad qu+(1-q)d=R.
$$

Giving each successive up move conditional [probability](../../../../../probability.md) $q$ defines an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q$, since every finite path has positive probability and $\mathbb E_Q[S_{r+1}\mid\mathcal F_r]=RS_r$.

For a [contingent claim](../../../../../contingent-claim.md) with successor values $V_u,V_d$ at a node of current stock value $s$, solve the two replication equations. The number of shares and current cash value are

$$
\Delta=\frac{V_u-V_d}{s(u-d)},\qquad C=\frac{uV_d-dV_u}{R(u-d)}.
$$

Then $\Delta us+RC=V_u$ and $\Delta ds+RC=V_d$, so the [replicating strategy](../../../../../replicating-strategy.md) costs

$$
V=\Delta s+C=R^{-1}\{qV_u+(1-q)V_d\}.
$$

Hold $C/B_r$ bank-account units over that period. Starting with the terminal payoff and applying these equations backwards supplies an adapted [self-financing strategy](../../../../../self-financing-portfolio.md) replicating every path-dependent [contingent claim](../../../../../contingent-claim.md). This proves [market completeness](../../../../../complete-market.md). A different claim price would permit an [arbitrage](../../../../../arbitrage.md) by buying the cheaper claim or replica and selling the dearer one. Iterating the backward pricing relation gives the unique [risk-neutral pricing](../../../../../risk-neutral-pricing.md) formula

$$
V_r=R^{-(n-r)}\mathbb E_Q[H\mid\mathcal F_r].
$$

The physical up probability affects real-world frequencies but does not enter this replication price.

For a terminal payoff $f(S_n)$, write $k=n-r$. Its current price is the restriction to the available nodes of the function

$$
g_r(s)=R^{-k}\sum_{j=0}^k\binom{k}{j}q^j(1-q)^{k-j}f(su^jd^{k-j}),\qquad s>0.
$$

If $f$ is [convex](../../../../../convex-function.md), each summand is [convex](../../../../../convex-function.md) in $s$ and each weight is positive; summing their defining convexity inequalities proves that $g_r$ is [convex](../../../../../convex-function.md). This provides an explicit [convex](../../../../../convex-function.md) extension between the actual stock nodes, so “convex on the nodes” is unambiguous. If $f$ is [strictly convex](../../../../../strictly-convex-function.md), each positive scaling preserves strict convexity, so $g_r$ is [strictly convex](../../../../../strictly-convex-function.md) as well.

For the [replicating portfolio in a binomial market](../../../../../replicating-portfolio-in-a-binomial-market.md), the stock holding is

$$
\Delta_r(s)=\frac{g_{r+1}(us)-g_{r+1}(ds)}{s(u-d)}.
$$

For $r+1<n$, let $F=g_{r+2}$. The next down and up holdings are the secant slopes of $F$ on the adjacent intervals with endpoints $d^2s,uds,u^2s$:

$$
\Delta_{r+1}(ds)=\frac{F(uds)-F(d^2s)}{ds(u-d)},\qquad
\Delta_{r+1}(us)=\frac{F(u^2s)-F(uds)}{us(u-d)}.
$$

For any [convex function](../../../../../convex-function.md) and $a<b<c$, its defining inequality at $b=(1-t)a+tc$ rearranges to $(F(b)-F(a))/(b-a)\leq(F(c)-F(b))/(c-b)$. The inequality is strict for a [strictly convex function](../../../../../strictly-convex-function.md). Applying this to the three stock values orders the two next holdings. Meanwhile the backward pricing relation gives, by subtracting its values at $us$ and $ds$,

$$
\Delta_r(s)=\frac{qu}{R}\Delta_{r+1}(us)+\frac{(1-q)d}{R}\Delta_{r+1}(ds).
$$

The coefficients are strictly positive and sum to one. Therefore the current share holding lies between the next two holdings:

$$
\boxed{\Delta_{r+1}(us)\geq\Delta_r(s)\geq\Delta_{r+1}(ds).}
$$

Both inequalities are strict for a [strictly convex](../../../../../strictly-convex-function.md) payoff. For an affine payoff the share holding is constant, explaining the required weak interpretation. These are numbers of shares, not the fraction of [portfolio wealth](../../../../../portfolio-wealth.md) invested in the [stock](../../../../../stock.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
