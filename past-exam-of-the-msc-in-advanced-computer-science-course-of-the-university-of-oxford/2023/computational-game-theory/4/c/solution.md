<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the usual [empty-coalition normalization](../../../../../empty-coalition-normalization.md) $v(\varnothing)=0$ for a [transferable utility game](../../../../../transferable-utility-game.md). Write $P_i=\{1,\ldots,i-1\}$, so the proposed [payoff](../../../../../payoff.md) is the [marginal contribution](../../../../../marginal-contribution.md)

$$
x_i=v(P_i\cup\{i\})-v(P_i).
$$

The vector is the [marginal contribution vector](../../../../../marginal-contribution-vector.md) for the natural player order.

First, [convex cooperative games](../../../../../convex-cooperative-game.md) have increasing [marginal contributions](../../../../../marginal-contribution.md). If $A\subseteq B$ and $i\notin B$, apply the defining [supermodular set function](../../../../../supermodular-set-function.md) inequality to $A\cup\{i\}$ and $B$:

$$
v(A\cup\{i\})+v(B)
\le v(B\cup\{i\})+v(A).
$$

Rearranging gives

$$
v(A\cup\{i\})-v(A)
\le v(B\cup\{i\})-v(B).
$$

The vector is efficient by a [telescoping sum](../../../../../telescoping-sum.md):

$$
\sum_{i=1}^{n}x_i
=\sum_{i=1}^{n}
\bigl(v(\{1,\ldots,i\})-v(\{1,\ldots,i-1\})\bigr)
=v(N)-v(\varnothing)=v(N).
$$

Now fix any [coalition](../../../../../coalition-game-theory.md) $T$. For each $i\in T$, its earlier members are $T\cap P_i\subseteq P_i$. Increasing [marginal contributions](../../../../../marginal-contribution.md) therefore give

$$
x_i\ge v((T\cap P_i)\cup\{i\})-v(T\cap P_i).
$$

Sum over the members of $T$ in increasing order. The right-hand side is another [telescoping sum](../../../../../telescoping-sum.md), now along the growing [coalition](../../../../../coalition-game-theory.md) $T$:

$$
\sum_{i\in T}x_i\ge v(T)-v(\varnothing)=v(T).
$$

Efficiency and these inequalities for every [coalition](../../../../../coalition-game-theory.md) are exactly the defining requirements of the [core of a cooperative game](../../../../../core-game-theory.md). Thus **$x$ belongs to the [core](../../../../../core-game-theory.md)**. The same proof works for any player ordering, not only the natural order.

The normalization is essential to the literal statement: the printed part does not explicitly state it. Without $v(\varnothing)=0$, take the constant [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) $v(T)=1$. It satisfies the displayed [convex cooperative game](../../../../../convex-cooperative-game.md) inequality with equality, but every proposed $x_i$ is zero, so efficiency fails when $N$ is nonempty. Under the standard normalized definition, the proof above establishes the intended result.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2023](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
