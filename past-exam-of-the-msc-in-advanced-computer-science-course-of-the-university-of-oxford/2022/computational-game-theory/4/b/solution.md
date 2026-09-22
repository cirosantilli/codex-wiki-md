<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the standard [empty-coalition normalization](../../../../../empty-coalition-normalization.md) $v(\varnothing)=0$. A [convex cooperative game](../../../../../convex-cooperative-game.md) has increasing [marginal contributions](../../../../../marginal-contribution.md): whenever $A\subseteq B$ and $i\notin B$,

$$
v(A\cup\{i\})-v(A)\le v(B\cup\{i\})-v(B).
$$

This follows from the [supermodular](../../../../../supermodular-set-function.md) inequality applied to $A\cup\{i\}$ and $B$. Fix a [permutation](../../../../../permutation.md) $\pi$ of all players, let $P_i$ be the players preceding $i$, and form its [marginal contribution vector](../../../../../marginal-contribution-vector.md)

$$
m_i^\pi=v(P_i\cup\{i\})-v(P_i).
$$

Summing along the full [permutation](../../../../../permutation.md) is a [telescoping sum](../../../../../telescoping-sum.md), so $\sum_{i\in N}m_i^\pi=v(N)$. For an arbitrary [coalition](../../../../../coalition-game-theory.md) $S$, list its members in their induced order $i_1,\ldots,i_k$, and put $S_j=\{i_1,\ldots,i_j\}$. Since $S_{j-1}\subseteq P_{i_j}$, increasing [marginal contributions](../../../../../marginal-contribution.md) give

$$
\sum_{i\in S}m_i^\pi\ge\sum_{j=1}^k\bigl(v(S_j)-v(S_{j-1})\bigr)=v(S).
$$

Thus every [marginal contribution vector](../../../../../marginal-contribution-vector.md) belongs to the [core](../../../../../core-game-theory.md). The vector of [Shapley values](../../../../../shapley-value.md) is exactly their uniform average over the $n!$ [permutations](../../../../../permutation.md), hence a [convex combination](../../../../../convex-combination.md). By the preceding part, that average is in the [core](../../../../../core-game-theory.md). This proves that **the [Shapley value](../../../../../shapley-value.md) allocation belongs to the [core](../../../../../core-game-theory.md) of a [convex cooperative game](../../../../../convex-cooperative-game.md)**, including every [coalition](../../../../../coalition-game-theory.md) constraint. It is the result [Shapley value belongs to the core of a convex game](../../../../../shapley-value-belongs-to-the-core-of-a-convex-game.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2022](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
