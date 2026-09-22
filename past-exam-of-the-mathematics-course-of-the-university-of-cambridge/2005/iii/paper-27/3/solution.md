<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [axiom of determinacy](../../../../../axiom-of-determinacy.md), $\mathsf{AD}$, says that every [infinite game of perfect information](../../../../../infinite-game-of-perfect-information.md) in which two players alternately choose [natural numbers](../../../../../natural-number.md) and Player I wins according to a specified payoff $A\subseteq\omega^\omega$ is a [determined infinite game](../../../../../determined-infinite-game.md). A [strategy](../../../../../strategy-in-an-infinite-game.md) specifies a move at every finite position where its player moves; it is winning if every compatible infinite play is won by that player.

Finite games are determined by [backward induction](../../../../../backward-induction.md). For infinite games, [open determinacy](../../../../../open-determinacy.md) has a direct proof. Let $T$ consist of the finite positions whose extension [cylinder sets](../../../../../cylinder-set.md) lie in the open payoff $A$. Build the [winning-position attractor in an infinite game](../../../../../winning-position-attractor-in-an-infinite-game.md) by [transfinite recursion](../../../../../transfinite-recursion.md): start with $T$, add an I-position if some successor has already entered, add a II-position if every successor has already entered, and take unions at limit stages. The process stabilizes because there are only countably many finite positions.

At a position in the attractor but outside $T$, I can choose a successor with strictly smaller entry rank, and every move of II has smaller entry rank. There is no infinite descending sequence of [ordinals](../../../../../ordinal.md), so I forces entry into $T$ and wins. Outside the attractor, every I-move stays outside it, while II can choose a successor outside it; that strategy avoids $T$ forever. Since $A$ is open, a play belongs to $A$ exactly when some prefix belongs to $T$. Thus II wins from outside the attractor. This proves determination for open payoffs; swapping the players proves it for closed payoffs too. The stronger [Borel determinacy theorem](../../../../../borel-determinacy-theorem.md) gives determination for every [Borel set](../../../../../borel-set.md) payoff, whereas $\mathsf{AD}$ asserts this for arbitrary payoffs.

To contradict $\mathsf{AD}$ from [choice](../../../../../axiom-of-choice.md), enumerate both players' strategies as $\langle\sigma_\alpha:\alpha<\mathfrak c\rangle$ and $\langle\tau_\alpha:\alpha<\mathfrak c\rangle$, where $\mathfrak c=2^{\aleph_0}$. There are $\mathfrak c$ strategies because the set of finite positions is countable; there are also $\mathfrak c$ plays following any fixed strategy because the other player's moves are arbitrary. At stage $\alpha$ of the [choice diagonalization of an undetermined game](../../../../../choice-diagonalization-of-an-undetermined-game.md), choose a fresh play $x_\alpha$ following $\sigma_\alpha$ and then a different fresh play $y_\alpha$ following $\tau_\alpha$, avoiding all earlier reservations. This is possible because fewer than $\mathfrak c$ plays have been reserved at every $\alpha<\mathfrak c$; regularity of $\mathfrak c$ is not required.

Set $A=\{y_\alpha:\alpha<\mathfrak c\}$. Every $\sigma_\alpha$ loses on $x_\alpha\notin A$, and every $\tau_\alpha$ loses on $y_\alpha\in A$. Thus neither player has a [winning strategy](../../../../../winning-strategy-in-an-infinite-game.md), and **AD and AC are inconsistent together.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
