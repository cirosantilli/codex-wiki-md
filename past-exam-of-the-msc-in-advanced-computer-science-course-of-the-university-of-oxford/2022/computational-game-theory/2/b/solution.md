<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent satisfied and unsatisfied goals by [payoffs](../../../../../payoff.md) one and zero. The second player's goal is an [exclusive or](../../../../../exclusive-or.md): it is true precisely when $q\ne r$, independently of $p$. The first goal is false only when all three [Boolean variables](../../../../../boolean-variable.md) are false. The resulting [payoff matrix](../../../../../payoff-matrix.md) is below; each boxed entry marks that player's [best response](../../../../../best-response.md) to the opposing [pure strategy](../../../../../pure-strategy.md), including ties:

$$
\begin{array}{c|cccc}
 &pq&p\bar q&\bar p q&\bar p\bar q\\\hline
r&(\boxed{1},0)&(\boxed{1},\boxed{1})&(\boxed{1},0)&(\boxed{1},\boxed{1})\\
\bar r&(\boxed{1},\boxed{1})&(\boxed{1},0)&(\boxed{1},\boxed{1})&(0,0)
\end{array}
$$

For player 1, choosing $r$ satisfies the goal against every opposing [pure strategy](../../../../../pure-strategy.md). Choosing $\bar r$ does equally well except against $\bar p\bar q$, where it does worse. Thus **$r$ is player 1's unique [dominant strategy](../../../../../dominant-strategy.md) in the weak sense**, and there is no [strictly dominant strategy](../../../../../strictly-dominant-strategy.md). The ties are why most first-player entries in both rows are boxed.

For player 2, either [pure strategy](../../../../../pure-strategy.md) with $q=0$ is a [best response](../../../../../best-response.md) against $r$, while either with $q=1$ is a [best response](../../../../../best-response.md) against $\bar r$. No one choice of $q$ works against both rows, so **player 2 has no [dominant strategy](../../../../../dominant-strategy.md)**, and **there is no [dominant-strategy equilibrium](../../../../../dominant-strategy-equilibrium.md)**. The value of $p$ does not affect player 2's own [payoff](../../../../../payoff.md).

The cells with both entries boxed give exactly four [pure strategy](../../../../../pure-strategy.md) [Nash equilibria](../../../../../nash-equilibrium.md):

$$
\boxed{(r,p\bar q),\quad(r,\bar p\bar q),\quad(\bar r,pq),\quad(\bar r,\bar p q).}
$$

All four give [payoffs](../../../../../payoff.md) $(1,1)$. In particular, the [weakly dominated](../../../../../weakly-dominated-strategy.md) choice $\bar r$ can occur in a [Nash equilibrium](../../../../../nash-equilibrium.md) because player 1 is already satisfied there and cannot strictly improve.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2022](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
