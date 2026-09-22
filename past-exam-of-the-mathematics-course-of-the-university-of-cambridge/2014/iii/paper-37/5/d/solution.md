<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**True, with the usual normalization $v(\varnothing)=0$.** For a [convex cooperative game](../../../../../../convex-cooperative-game.md), the [supermodular](../../../../../../supermodular-set-function.md) inequality implies increasing [marginal contributions](../../../../../../marginal-contribution.md): if $A\subseteq B$ and $i\notin B$, apply it to $A\cup\{i\}$ and $B$ to obtain

$$
v(A\cup\{i\})-v(A)\le v(B\cup\{i\})-v(B).
$$

Fix an ordering $\pi$ and let $P_i$ be the set of players before $i$. Its [marginal contribution vector](../../../../../../marginal-contribution-vector.md) is $m_i^\pi=v(P_i\cup\{i\})-v(P_i)$. Summing in order telescopes to $\sum_i m_i^\pi=v(N)$. For any [coalition](../../../../../../coalition-game-theory.md) $S$, $S\cap P_i\subseteq P_i$, so increasing marginals give

$$
\sum_{i\in S}m_i^\pi\ge\sum_{i\in S}\bigl(v((S\cap P_i)\cup\{i\})-v(S\cap P_i)\bigr)=v(S).
$$

These are exactly the efficiency and [coalition](../../../../../../coalition-game-theory.md) constraints of the [core of a cooperative game](../../../../../../core-game-theory.md). Thus every [marginal contribution](../../../../../../marginal-contribution.md) vector is in the [core](../../../../../../core-game-theory.md). The [core](../../../../../../core-game-theory.md) is a [convex set](../../../../../../convex-set.md), being an intersection of linear [half-spaces](../../../../../../half-space.md) and an efficiency [hyperplane](../../../../../../hyperplane.md). The [Shapley value](../../../../../../shapley-value.md) is the average of the [marginal contribution](../../../../../../marginal-contribution.md) vectors over all orderings, so it too lies in the [core](../../../../../../core-game-theory.md). This proves [Shapley value belongs to the core of a convex game](../../../../../../shapley-value-belongs-to-the-core-of-a-convex-game.md), without needing a separate existence theorem for the [core](../../../../../../core-game-theory.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
