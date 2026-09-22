<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write column $j$ as $((a_j,c_j),(b_j,d_j))^T$, where the row player's binary [payoff](../../../../../payoff.md) is first. Suppose, for a contradiction, there is no pure [Nash equilibrium](../../../../../nash-equilibrium.md).

The column player's maximum [payoff](../../../../../payoff.md) in the top row must be one. Otherwise every column would be its [best response](../../../../../best-response.md) there. To avoid a top-row equilibrium, every column would then need $a_j=0,b_j=1$. But a column maximizing $d_j$ would immediately give a bottom-row equilibrium. The same reasoning with rows exchanged shows that the maximum bottom-row column [payoff](../../../../../payoff.md) is also one.

Choose a column with $c_j=1$. To avoid a top-row equilibrium, it must have $a_j=0,b_j=1$. It cannot also have $d_j=1$, because its bottom cell would then be an equilibrium. Hence this column is $((0,1),(1,0))^T$, the specified second column type. Exchanging rows forces a column $((1,0),(0,1))^T$, the specified first type.

Thus **absence of a pure equilibrium forces both forbidden column types to occur**. If the given game omits them, this is a contradiction, proving existence of a pure [Nash equilibrium](../../../../../nash-equilibrium.md). The argument actually proves the stronger statement that omitting either one of the two types suffices.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
