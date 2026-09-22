<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Both players can guarantee $k$ by part (d), so at any [Nash equilibrium](../../../../../nash-equilibrium.md) each must receive at least $k$. Their [payoffs](../../../../../payoff.md) sum to $2k$, forcing both equilibrium [payoffs](../../../../../payoff.md) to equal $k$.

Moreover, an equilibrium action must itself have the maxmin guarantee $k$. If a player's chosen action allowed an opposing response that reduced its [payoff](../../../../../payoff.md) below $k$, that response would give the opponent more than $k$, a profitable [unilateral deviation](../../../../../unilateral-deviation.md). Thus both equilibrium sites belong to the central [set](../../../../../set-split.md) identified in part (d).

Conversely, if both choose from that central [set](../../../../../set-split.md), each chosen action guarantees $k$. Neither can improve above $k$, because the other player's fixed central action still guarantees the other player $k$. Consequently, **all pure [Nash equilibria](../../../../../nash-equilibrium.md) are**

$$
\boxed{\begin{cases}((k+1)/2,(k+1)/2),&k\text{ odd},\\(x,y)\in\{k/2,k/2+1\}^2,&k\text{ even}.\end{cases}}
$$

For even $k$, this includes both co-located central profiles and both orders of the two distinct central sites.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
