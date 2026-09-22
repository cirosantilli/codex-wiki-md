<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**$G_1$ cannot have an [induced subgraph game](../../../../../induced-subgraph-game.md) representation. $G_2$ is represented by a weighted triangle with edge weights $w_{12}=2$, $w_{13}=3$, $w_{23}=3$, and has [Shapley value](../../../../../shapley-value.md) vector $(5/2,5/2,3)$.**

In an [induced subgraph game](../../../../../induced-subgraph-game.md), players are [graph vertices](../../../../../vertex-graph-theory.md) and a [coalition](../../../../../coalition-game-theory.md) receives the sum of the weights of [graph edges](../../../../../edge-of-a-graph.md) whose two endpoints lie in it. Therefore each two-player [coalition](../../../../../coalition-game-theory.md) determines the corresponding edge weight. For $G_1$ these weights would have to be $2,6,3$, making the grand [coalition](../../../../../coalition-game-theory.md) worth $2+6+3=11$, whereas its actual value is $15$. No other edge weights can repair that discrepancy without changing a two-player [coalition](../../../../../coalition-game-theory.md)'s value. Even a convention allowing vertex weights would not help: its singleton values force all such weights to zero.

For $G_2$, the stated weighted [graph triangle](../../../../../triangle-in-a-graph.md) has grand [coalition](../../../../../coalition-game-theory.md) value $2+3+3=8$ and reproduces all three pair values. Empty and singleton [coalitions](../../../../../coalition-game-theory.md) contain no [graph edges](../../../../../edge-of-a-graph.md), so their values are zero. This verifies all eight [coalitions](../../../../../coalition-game-theory.md) and supplies the complete representation.

To compute the [Shapley value](../../../../../shapley-value.md), reveal players in a uniformly random [permutation](../../../../../permutation.md). An edge's weight contributes to an endpoint's [marginal contribution](../../../../../marginal-contribution.md) precisely when the other endpoint appeared earlier. Each endpoint is later with [probability](../../../../../probability.md) $1/2$, independently of where the third player appears. Linearity of the [expected value](../../../../../expected-value-split.md) therefore splits each edge weight equally between its two endpoints:

$$
\boxed{\phi_1=\frac{2+3}{2}=\frac52,\quad
\phi_2=\frac{2+3}{2}=\frac52,\quad
\phi_3=\frac{3+3}{2}=3.}
$$

The values sum to $8=v_2(N)$, as required by the [Shapley value](../../../../../shapley-value.md)'s efficiency property. This is the general [Shapley value of an induced subgraph game](../../../../../shapley-value-of-an-induced-subgraph-game.md) formula, not an assumption that all three players are symmetric: player $3$ has a different incident-weight total.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
