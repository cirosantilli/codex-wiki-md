<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**No. Two positive [self-loops](../../../../../loop-graph-theory.md) and one negative [edge](../../../../../edge-of-a-graph.md) give a [simple cooperative game](../../../../../simple-cooperative-game.md) with an empty [core of a cooperative game](../../../../../core-game-theory.md).** Give players $1,2$ loop weights $\ell_1=\ell_2=1$, put $w_{12}=-1$, and give every other loop and [edge](../../../../../edge-of-a-graph.md) weight zero. For a [coalition](../../../../../coalition-game-theory.md) $S$,

$$
v(S)=\mathbf1_{\{1\in S\}}+\mathbf1_{\{2\in S\}}
-\mathbf1_{\{\{1,2\}\subseteq S\}}
=\mathbf1_{\{S\cap\{1,2\}\ne\varnothing\}}.
$$

Thus a [coalition](../../../../../coalition-game-theory.md) wins exactly when it contains player $1$ or player $2$. This is monotone, has values in $\{0,1\}$, and satisfies $v(\varnothing)=0,v(N)=1$. Extra players for any $n\ge3$ do not alter any [coalition](../../../../../coalition-game-theory.md) value.

The [core](../../../../../core-game-theory.md) singleton inequalities would require $x_1\ge1$, $x_2\ge1$ and $x_i\ge0$ for every other player, while efficiency requires $\sum_i x_i=1$. These requirements are inconsistent. Equivalently, the two disjoint winning singleton [coalitions](../../../../../coalition-game-theory.md) leave no [veto player](../../../../../veto-player.md). Signed weights are essential to this particular representation and are permitted in the [induced subgraph game](../../../../../induced-subgraph-game.md) model.

## ↑ Ancestors (11)

1. [E](../e.md)
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
