<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [security level payoff](../../../../../../security-level-payoff.md) maximizes what a player guarantees against the opponent. Let $p$ be the row player's probability of the first action. Its guaranteed payoff is

$$
\min\{3-3p,2+2p\}.
$$

The decreasing and increasing terms cross at $p=1/5$, attaining $d_1=12/5$; moving either way lowers the smaller term. For the column player, any mixture has zero payoff against the first row, while its second-row payoff is nonnegative. Therefore $d_2=0$ and

$$
d=(12/5,0).
$$

The feasible set is the [convex hull](../../../../../../convex-hull.md) of the four joint pure-action payoff vectors. Its upper [Pareto frontier](../../../../../../pareto-frontier.md) connects $(4,0)$ to $(3,2)$ to $(2,3)$. Write the row payoff as $u$ and column payoff as $v$. On the first [Pareto frontier](../../../../../../pareto-frontier.md) segment, $v=8-2u$ for $3\leq u\leq4$. The [Nash product](../../../../../../nash-product.md) is

$$
(u-12/5)(8-2u),
$$

a concave quadratic with [derivative](../../../../../../derivative.md) $64/5-4u$, maximized at $u=16/5$, $v=8/5$, giving product $32/25$. On the portion of the other [Pareto frontier](../../../../../../pareto-frontier.md) segment satisfying [bargaining individual rationality](../../../../../../bargaining-individual-rationality.md), $12/5\leq u\leq3$ and $v=5-u$. Its product [derivative](../../../../../../derivative.md) $37/5-2u$ is positive throughout, so its largest product is $6/5$ at $(3,2)$, smaller than $32/25$. All dominated points can be discarded by [Pareto efficiency](../../../../../../pareto-efficiency.md). Consequently

$$
\boxed{N(F,d)=(16/5,8/5).}
$$

This payoff is implemented by a [correlated payoff lottery](../../../../../../lottery-over-joint-action-profiles.md) choosing the payoff $(4,0)$ with probability $1/5$ and $(3,2)$ with probability $4/5$. The [convex hull](../../../../../../convex-hull.md) permits such lotteries over joint outcomes; it is not restricted to independent [mixed strategies](../../../../../../mixed-strategy.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
