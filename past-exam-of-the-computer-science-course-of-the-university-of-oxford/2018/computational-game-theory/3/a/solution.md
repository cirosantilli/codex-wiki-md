<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an $n$-player [transferable utility game](../../../../../transferable-utility-game.md) with $v(\varnothing)=0$, the [Shapley value](../../../../../shapley-value.md) is

$$
\boxed{\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}\frac{|S|!\,(n-|S|-1)!}{n!}\left(v(S\cup\{i\})-v(S)\right).}
$$

It averages player $i$'s [marginal contribution](../../../../../marginal-contribution.md) over uniformly random orders of all players. Exactly $|S|!(n-|S|-1)!$ of the $n!$ [permutations](../../../../../permutation.md) put precisely $S$ before $i$. For a [cooperative cost game](../../../../../cooperative-cost-game.md), apply the same linear formula to the cost function; the result represents payments instead of distributed benefits.

## ↑ Ancestors (11)

1. [A](../a.md)
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
