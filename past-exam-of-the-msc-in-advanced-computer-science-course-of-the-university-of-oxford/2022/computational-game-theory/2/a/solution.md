<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Reading the lower-left number in each source cell as player 1's [payoff](../../../../../payoff.md), against an opponent playing $A$ the player's own [payoffs](../../../../../payoff.md) from $A,B$ are $y,0$; against $B$ they are $x,x/2$. For $x>0$, identify $A$ with aggressive defection and $B$ with yielding cooperation. The standard [payoffs](../../../../../payoff.md) then have values

$$
T=x,\qquad R=x/2,\qquad S=0,\qquad P=y.
$$

The [prisoner's dilemma](../../../../../prisoner-s-dilemma.md) ordering $T>R>P>S$ holds precisely for **$x>0$ and $0<y<x/2$** with this labeling. For example, $x=4,y=1$ gives $T=4,R=2,P=1,S=0$. Each player then has the [strictly dominant strategy](../../../../../strictly-dominant-strategy.md) $A$, although $(B,B)$ gives both a larger [payoff](../../../../../payoff.md) than $(A,A)$. Here $2R=T+S$ as well, so the optional weak aggregate-payoff condition is met with equality.

For the [Chicken payoff ordering](../../../../../chicken-payoff-ordering.md), the collision outcome must be worse than yielding to an aggressive opponent: $T>R>S>P$. This holds for **$x>0$ and $y<0$**, for example $x=4,y=-1$. Against $B$, the [best response](../../../../../best-response.md) is $A$ because $x>x/2$; against $A$, it is $B$ because $0>y$. Consequently $(A,B)$ and $(B,A)$ are the two [pure strategy](../../../../../pure-strategy.md) [Nash equilibria](../../../../../nash-equilibrium.md), and mutual aggression is the worst outcome for both.

If action names may be exchanged, there is another [prisoner's dilemma](../../../../../prisoner-s-dilemma.md) region: take $A$ as cooperation and $B$ as defection. Then $(T,R,P,S)=(0,y,x/2,x)$, so **$x<0$ and $x/2<y<0$** also work, for example $x=-4,y=-1$. This relabeling explains why the first displayed region is not a necessary condition without an action convention. Equality at any of these boundaries destroys the strict ordering.

## ↑ Ancestors (11)

1. [A](../a.md)
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
