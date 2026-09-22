<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $c(\varnothing)=0$. For nonempty [coalitions](../../../../../coalition-game-theory.md), the runway required by a union is the longer of the two required runways, so

$$
c(S\cup T)=\max(c(S),c(T))\leq c(S)+c(T).
$$

The inequality uses nonnegative costs and also holds when either coalition is empty. Thus **the cost function is subadditive**, in particular for the stated disjoint [coalitions](../../../../../coalition-game-theory.md). A [subadditive cost game](../../../../../subadditive-cost-game.md) becomes a [superadditive coalitional game](../../../../../superadditive-coalitional-game.md) after changing signs to $v=-c$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
