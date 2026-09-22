<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes; without [self-loops](../../../../../loop-graph-theory.md), such a nontrivial [simple cooperative game](../../../../../simple-cooperative-game.md) has exactly one positive [edge](../../../../../edge-of-a-graph.md), of weight $1$.** For each pair,

$$
w_{ij}=v(\{i,j\})\in\{0,1\},
$$

because singleton and loop contributions are zero. Summing all [edge weights](../../../../../edge-weight.md) gives $v(N)=1$, so precisely one unordered pair $\{a,b\}$ has weight $1$, and all other pairs have weight zero.

Thus the [winning coalitions](../../../../../winning-coalition.md) are exactly those containing both $a$ and $b$. For any $0\le\lambda\le1$, set

$$
\boxed{x_a=\lambda,\quad x_b=1-\lambda,\quad x_i=0\quad(i\notin\{a,b\}).}
$$

This [payoff](../../../../../payoff.md) [vector](../../../../../vector.md) is efficient, since $\sum_i x_i=v(N)=1$. Every [winning coalition](../../../../../winning-coalition.md) receives $1$ and every losing [coalition](../../../../../coalition-game-theory.md) receives a nonnegative total, so all inequalities $x(S)\ge v(S)$ hold. Hence it belongs to the [core of a cooperative game](../../../../../core-game-theory.md).

In fact these are all [core](../../../../../core-game-theory.md) allocations. Singleton conditions require $x_i\ge0$, and the winning pair requires $x_a+x_b\ge1$; efficiency then forces equality and zero [payoffs](../../../../../payoff.md) outside the pair. The endpoints are both [veto players](../../../../../veto-player.md), consistent with the general characterization of the [core of a simple cooperative game](../../../../../core-of-a-simple-cooperative-game.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
