<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [axiom of determinacy](../../../../../axiom-of-determinacy.md), abbreviated AD, asserts that every length-$\omega$ [infinite game of perfect information](../../../../../infinite-game-of-perfect-information.md) in which the two players alternately choose [natural numbers](../../../../../natural-number.md) is determined. For a payoff [set](../../../../../set-split.md) $A\subseteq\omega^\omega$, player I wins exactly when the completed play belongs to $A$. A [strategy](../../../../../strategy-in-an-infinite-game.md) specifies the next move at every finite position where its player is to move; determination means that one player has a [winning strategy](../../../../../winning-strategy-in-an-infinite-game.md).

Finite games are determined by backward induction, choosing the least move leading to a guaranteed win when several are available. In [ZF](../../../../../zermelo-fraenkel-set-theory.md) one can also prove [open determinacy](../../../../../open-determinacy.md), hence determinacy for closed payoffs. Here is the full open-payoff argument. Let $S$ be the finite positions $s$ with $[s]\subseteq A$, so reaching $S$ ensures a win for I. Starting with $W_0=S$, repeatedly add an I-position with some child already in $W$, and a II-position with every child already in $W$; take [unions](../../../../../set-union.md) at limit stages. This increasing process stabilizes because the [set](../../../../../set-split.md) of finite positions is a [set](../../../../../set-split.md): continuing strict enlargement through its Hartogs number would choose distinct new positions, contradicting that bound. Assign to each admitted position its least entry stage.

At an I-position in the final $W$, choose the least child of smaller entry stage. At a II-position in $W\setminus S$, every child has smaller entry stage. A play following this I-strategy cannot remain outside $S$ forever, since that would give an infinite strictly descending [sequence](../../../../../sequence.md) of [ordinals](../../../../../ordinal.md). It reaches $S$ and wins. Outside $W$, every child of an I-position remains outside $W$, and a II-position has at least one child outside $W$. Player II chooses the least such child. The play never reaches $S$, so it cannot belong to the [open set](../../../../../open-set.md) $A$. The initial position is either inside or outside $W$, proving determination. For a closed payoff apply the same argument to the open complementary payoff for the other player, with the appropriate player assigned to each level. None of these [strategies](../../../../../strategy-in-an-infinite-game.md) needs a choice principle because moves are [natural numbers](../../../../../natural-number.md) and least available moves are definable.

To refute simultaneous AD and the [axiom of choice](../../../../../axiom-of-choice.md), assume choice and [well-order](../../../../../well-order.md) all [strategies](../../../../../strategy-in-an-infinite-game.md) of either player in length $\mathfrak c=2^{\aleph_0}$. There are exactly $\mathfrak c$ [strategies](../../../../../strategy-in-an-infinite-game.md) for each player, and any fixed [strategy](../../../../../strategy-in-an-infinite-game.md) has exactly $\mathfrak c$ compatible plays, since the opponent's successive moves are arbitrary. At stage $\alpha<\mathfrak c$, choose two fresh plays: $x_\alpha$ compatible with I's $\alpha$th [strategy](../../../../../strategy-in-an-infinite-game.md), and $y_\alpha$ compatible with II's $\alpha$th [strategy](../../../../../strategy-in-an-infinite-game.md). Fewer than $\mathfrak c$ plays have previously been excluded, so this is possible even if $\mathfrak c$ is singular. Put $A=\{y_\alpha:\alpha<\mathfrak c\}$. No $x_\alpha$ ever enters $A$. I's $\alpha$th [strategy](../../../../../strategy-in-an-infinite-game.md) loses on $x_\alpha$, and II's $\alpha$th [strategy](../../../../../strategy-in-an-infinite-game.md) loses on $y_\alpha$. Thus this game has no [winning strategy](../../../../../winning-strategy-in-an-infinite-game.md) for either player, and

$$
\boxed{\mathsf{AD}\ \Longrightarrow\ \neg\mathsf{AC}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
