<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the two-by-two [payoff](../../../../../payoff.md) entries visible in the original PDF. If $q$ is the probability that II uses its first action, I's expected [payoffs](../../../../../payoff.md) from its two [pure strategies](../../../../../pure-strategy.md) are $4-q$ and $2q$. Their difference $4-3q$ is strictly positive for every $q\in[0,1]$. Thus I's first action [strict dominance](../../../../../strict-dominance.md) its second, and every [Nash equilibrium](../../../../../nash-equilibrium.md) has I use the first action with probability one. Against that action, II receives 8 from its first action and 4 from its second, so its first action is uniquely optimal. Therefore

$$
\boxed{\text{the only equilibrium pair is }(I_1,II_1),\quad\text{with payoffs }(3,8).}
$$

This excludes nontrivial mixed equilibria as well as the other pure pairs.

For the [maximin bargaining solution](../../../../../maximin-bargaining-solution.md), first compute the two [security level payoffs](../../../../../security-level-payoff.md). If I uses its first action with probability $p$, its [payoffs](../../../../../payoff.md) against II's two [pure strategies](../../../../../pure-strategy.md) are $2+p$ and $4p$. Both increase with $p$, so its best worst-case [payoff](../../../../../payoff.md) is attained at $p=1$ and is $d_1=3$. If II uses its first action with probability $q$, its [payoffs](../../../../../payoff.md) against I's two actions are $4+4q$ and $6-6q$. The lower of these is maximized at their intersection,

$$
q=\frac15,\qquad d_2=\frac{24}{5}.
$$

These are separate security calculations, not the expected [payoffs](../../../../../payoff.md) from a pair of security strategies.

Cooperation permits jointly chosen lotteries, giving the [convex hull](../../../../../convex-hull.md) of the four [payoff](../../../../../payoff.md). The [vector](../../../../../vector.md) $(3,8)$ dominates $(2,0)$ and $(0,6)$, so the [Pareto frontier](../../../../../pareto-frontier.md) is the segment from $(3,8)$ to $(4,4)$, with equation $v=20-4u$. Individual rationality relative to $d=(3,24/5)$ restricts this to

$$
3\le u\le\frac{19}{5},\qquad v=20-4u.
$$

On this [negotiation set](../../../../../negotiation-set-in-two-person-bargaining.md), the [Nash product](../../../../../nash-product.md) is

$$
P(u)=(u-3)\left(\frac{76}{5}-4u\right),\qquad
P'(u)=\frac{136}{5}-8u,\quad P''(u)=-8.
$$

Its unique maximizer is interior, giving

$$
\boxed{(u_*,v_*)=\left(\frac{17}{5},\frac{32}{5}\right).}
$$

One implementing binding agreement always uses I's first action and uses II's first action with probability $3/5$, its second with probability $2/5$. This agreement raises both [payoffs](../../../../../payoff.md) above their security levels, but II receives $32/5<8$, less than at the noncooperative equilibrium. Thus **player II prefers the noncooperative game under the specified maximin bargaining rule**. The cooperative feasible set contains the equilibrium [payoff](../../../../../payoff.md); it is the particular arbitration rule, not an inability to cooperate at that [payoff](../../../../../payoff.md), that produces II's lower allocation.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
