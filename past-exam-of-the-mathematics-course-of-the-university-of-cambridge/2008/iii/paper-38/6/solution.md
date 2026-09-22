<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a [finite game](../../../../../finite-game.md), a profile of independent [mixed strategies](../../../../../mixed-strategy.md) $\sigma=(\sigma_1,\ldots,\sigma_n)$ is a [Nash equilibrium](../../../../../nash-equilibrium.md) if no player can improve their expected payoff by changing only their own [mixed strategy](../../../../../mixed-strategy.md). In symbols,

$$
U_a(\sigma_a,\sigma_{-a})\geq U_a(\tau_a,\sigma_{-a})
\quad\text{for every player }a\text{ and every strategy }\tau_a.
$$

Because expectation is linear in a player's own [mixed strategy](../../../../../mixed-strategy.md), checking this inequality for all their [pure strategies](../../../../../pure-strategy.md) suffices. Nothing requires the players' payoffs to sum to zero.

For the [symmetric finite game](../../../../../symmetric-finite-game.md), write $e_i(p)=e(i,p)$ and $\bar e(p)=\sum_i p_i e_i(p)$. Each $e_i(p)$ is a polynomial in the opponents' independent probabilities and therefore continuous on the [probability simplex](../../../../../probability-simplex.md) $\Delta=\{p\geq0:\sum_i p_i=1\}$. Put

$$
r_i(p)=\max(0,e_i(p)-\bar e(p)),\qquad
S(p)=\sum_i r_i(p),\qquad
F_i(p)=\frac{p_i+r_i(p)}{1+S(p)}.
$$

This continuous map has nonnegative coordinates summing to one, so it maps the compact [convex set](../../../../../convex-set.md) $\Delta$ into itself. The [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) gives $p=F(p)$. At that fixed point $r_i=p_iS$. If $S>0$, every $i$ in the [strategy support](../../../../../strategy-support.md) has $r_i>0$ and therefore $e_i(p)>\bar e(p)$. But

$$
\sum_i p_i(e_i(p)-\bar e(p))=0,
$$

whereas every supported term would be strictly positive, a contradiction. Thus $S=0$, all pure payoffs are at most $\bar e(p)$, and their weighted average equals $\bar e(p)$. Every supported [pure strategy](../../../../../pure-strategy.md) is consequently a [best response](../../../../../best-response.md) to the common opposing [mixed strategy](../../../../../mixed-strategy.md). **The profile in which every player uses $p$ is a symmetric Nash equilibrium.** This proves the [gain-map proof of symmetric equilibrium](../../../../../gain-map-proof-of-symmetric-equilibrium.md) for any finite number of players, including boundary fixed points of the [probability simplex](../../../../../probability-simplex.md).

In the [least unique bid auction](../../../../../least-unique-bid-auction.md), let $p$ be the common [probability](../../../../../probability.md) of bid 1. Bidding 1 wins only when the other two bids are both 2, and its winning payoff is $3-1=2$. Bidding 2 wins only when the other two bids are both 1, and its winning payoff is $3-2=1$. Hence the two expected payoffs are

$$
e_1(p)=2(1-p)^2,\qquad e_2(p)=p^2.
$$

Neither symmetric [pure strategy](../../../../../pure-strategy.md) profile is an equilibrium: against two bids of 1 a deviation to 2 earns 1 instead of 0, and against two bids of 2 a deviation to 1 earns 2 instead of 0. An interior [symmetric equilibrium](../../../../../symmetric-equilibrium.md) must make the two expected payoffs equal. Solving $2(1-p)^2=p^2$ leaves just one root in $(0,1)$, giving

$$
\boxed{p=2-\sqrt2\text{ for bid 1},\qquad1-p=\sqrt2-1\text{ for bid 2}.}
$$

The expected payoff to each player is $p^2=6-4\sqrt2$.

To count all nonsymmetric [Nash equilibria](../../../../../nash-equilibrium.md), let $p_i$ be player $i$'s [probability](../../../../../probability.md) of bidding 1. The difference between their expected payoffs from bids 1 and 2 is

$$
\Delta_i=2(1-p_j)(1-p_k)-p_jp_k
=2-2p_j-2p_k+p_jp_k.
$$

The [best response](../../../../../best-response.md) conditions are $p_i=1$ when $\Delta_i>0$, $p_i=0$ when $\Delta_i<0$, and arbitrary $p_i$ when $\Delta_i=0$.

For any $0\leq t\leq1$, the profile $(p_1,p_2,p_3)=(1,0,t)$ satisfies these conditions: $\Delta_1=2(1-t)\geq0$, $\Delta_2=-t\leq0$, and $\Delta_3=0$. Thus every permutation of this profile is a [Nash equilibrium](../../../../../nash-equilibrium.md). At $t=0,1$ these give the six pure profiles with at least one bid of each kind; for $0<t<1$, one player mixes freely and the other two use opposite [pure strategies](../../../../../pure-strategy.md).

There are no other nonsymmetric equilibria. If all three probabilities are interior, every $\Delta_i$ must vanish. Subtracting two such equations gives

$$
\Delta_1-\Delta_2=(p_1-p_2)(2-p_3)=0.
$$

Since $2-p_3>0$, all probabilities are equal, yielding the symmetric solution already found. If exactly two players mix and the third uses bid 2, either mixer strictly prefers bid 1 because $\Delta=2(1-p_j)>0$. If the third uses bid 1, either mixer strictly prefers bid 2 because $\Delta=-p_j<0$. Both cases are impossible. If exactly one player mixes, their indifference requires the other players to use opposite bids. Finally, with no mixing, the all-equal pure profiles fail and the remaining six satisfy the [best response](../../../../../best-response.md) conditions.

Consequently the complete [Nash equilibrium](../../../../../nash-equilibrium.md) set consists of the single symmetric mixed profile together with the six closed one-parameter families given by permutations of $(1,0,t)$. Their endpoints overlap at the six pure equilibria. In particular,

$$
\boxed{\text{there are uncountably infinitely many nonsymmetric equilibria}.}
$$

Counting only the six pure ones would miss the interior points of these families in the [two-bid three-player least unique bid auction](../../../../../two-bid-three-player-least-unique-bid-auction.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
