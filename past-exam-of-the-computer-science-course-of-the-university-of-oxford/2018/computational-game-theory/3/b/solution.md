<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take three players and define the [simple cooperative game](../../../../../simple-cooperative-game.md)

$$
v(S)=\begin{cases}1,&1\in S\text{ and }S\cap\{2,3\}\ne\varnothing,\\0,&\text{otherwise}.\end{cases}
$$

It is a [superadditive coalitional game](../../../../../superadditive-coalitional-game.md): two disjoint [coalitions](../../../../../coalition-game-theory.md) cannot both have value one because each would need player 1. If one has value one, their union does too; if neither does, the desired inequality is immediate.

The vector $(1,0,0)$ belongs to the [core of a cooperative game](../../../../../core-game-theory.md). More strongly, it is the unique core vector: singleton constraints give nonnegative coordinates, efficiency gives sum one, and the value-one coalitions $\{1,2\}$ and $\{1,3\}$ force $x_3=x_2=0$.

In a random player ordering, player 1 is pivotal unless it comes first, giving [Shapley value](../../../../../shapley-value.md) $2/3$. Player 2 is pivotal only in order $1,2,3$, and player 3 only in order $1,3,2$. Thus

$$
\boxed{\phi=(2/3,1/6,1/6),\qquad\operatorname{Core}(v)=\{(1,0,0)\}.}
$$

The coalition $\{1,2\}$ receives only $5/6<1$, so the [Shapley value](../../../../../shapley-value.md) is outside the [core](../../../../../core-game-theory.md). This proves that [superadditivity and nonempty core do not imply Shapley stability](../../../../../superadditivity-and-nonempty-core-do-not-imply-shapley-stability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
