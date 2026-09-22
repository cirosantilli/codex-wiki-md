<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $A\subseteq\omega^\omega$, let the players alternately choose natural numbers, producing $x\in\omega^\omega$; I wins exactly when $x\in A$. A [strategy](../../../../../../strategy-in-an-infinite-game.md) assigns a move to each finite position at which its player moves. It is winning if every compatible completed play is won by that player. A game is determined when one player has a [winning strategy](../../../../../../winning-strategy-in-an-infinite-game.md). The [axiom of determinacy](../../../../../../axiom-of-determinacy.md) is

$$
\boxed{\mathsf{AD}:\quad\text{every }A\subseteq\omega^\omega\text{ gives a determined game}.}
$$

We can prove determinacy for open and closed payoffs, including clopen payoffs; finite games are covered by backward [induction](../../../../../../mathematical-induction.md). Here is the full open-payoff argument. For an open $A$, let $W_0$ consist of finite positions whose entire cylinder of continuations is contained in $A$. Recursively put

$$
W_{\alpha+1}=W_\alpha\cup\{p:\text{I moves at }p\text{ and some }p^\frown n\in W_\alpha\}
\cup\{p:\text{II moves at }p\text{ and every }p^\frown n\in W_\alpha\},
$$

and take unions at limits. Since positions form a [set](../../../../../../set-split.md), this process reaches a fixed point $W$. More explicitly, a strict increase at each stage would assign a distinct position to each stage beyond the Hartogs bound of the position [set](../../../../../../set-split.md), which is impossible; for natural-number moves the least newly added position in a fixed enumeration makes that assignment explicit.

If the initial position belongs to $W$, I can win. At an I-position first added at a successor stage, choose the least move to a position of smaller first-entry rank. At an II-position first added at a successor stage, every successor already has smaller rank. A play following this [strategy](../../../../../../strategy-in-an-infinite-game.md) cannot have an infinite strictly descending [sequence](../../../../../../sequence.md) of [ordinal](../../../../../../ordinal.md) ranks, so reaches $W_0$ in finitely many steps; all its further continuations lie in $A$. If the initial position is outside $W$, II keeps the play outside $W$: at an I-position no successor is in $W$, and at an II-position at least one successor is outside $W$, so II chooses the least such move. The play never reaches a winning prefix. Since $A$ is open, membership in $A$ would have been certified by some finite prefix, so the resulting play is outside $A$. Thus **every open game is determined**. Applying this argument to the open complement of a closed payoff, with the players' objectives interchanged, proves closed determinacy too. The argument needs no choice of moves beyond taking the least available natural number.

To refute [AD](../../../../../../axiom-of-determinacy.md) under [AC](../../../../../../axiom-of-choice.md), first use binary moves. There are $\mathfrak c=2^{\aleph_0}$ [strategies](../../../../../../strategy-in-an-infinite-game.md) for each player, since its positions form a [countable](../../../../../../countable-set.md) [set](../../../../../../set-split.md). Enumerate them as $(\sigma_\alpha)_{\alpha<\mathfrak c}$ and $(\tau_\alpha)_{\alpha<\mathfrak c}$. Each fixed [strategy](../../../../../../strategy-in-an-infinite-game.md) admits exactly $\mathfrak c$ compatible plays: the other player's arbitrary binary [sequence](../../../../../../sequence.md) determines the completed play injectively. Recursively choose a play $u_\alpha$ following $\sigma_\alpha$ and a play $v_\alpha$ following $\tau_\alpha$, each different from all earlier reservations and from each other. This is possible because at stage $\alpha$ fewer than $\mathfrak c$ plays have been reserved. No regularity assumption on $\mathfrak c$ is used: every [ordinal](../../../../../../ordinal.md) $\alpha<\mathfrak c$ has cardinality below $\mathfrak c$, and doubling an infinite smaller [cardinal](../../../../../../cardinal-number.md) does not reach $\mathfrak c$.

[Set](../../../../../../set-split.md) $B=\{v_\alpha:\alpha<\mathfrak c\}\subseteq2^\omega$. [Strategy](../../../../../../strategy-in-an-infinite-game.md) $\sigma_\alpha$ loses on $u_\alpha\notin B$, while $\tau_\alpha$ loses on $v_\alpha\in B$. Thus this binary game is undetermined. Turn it into a natural-number game by declaring that the first player to play a number outside $\{0,1\}$ loses. Formally its I-payoff is

$$
A=B\cup\{x\in\omega^\omega:\text{the first }n\text{ with }x(n)>1\text{ is odd}\}.
$$

A [winning strategy](../../../../../../winning-strategy-in-an-infinite-game.md) in this game could not prescribe an illegal move after a compatible legal history, since the opponent could thereby win. Its restriction to legal histories would therefore give a winning binary [strategy](../../../../../../strategy-in-an-infinite-game.md), contradicting the construction. Hence the [choice diagonalization of an undetermined game](../../../../../../choice-diagonalization-of-an-undetermined-game.md) proves

$$
\boxed{\mathsf{AC}\Longrightarrow\neg\mathsf{AD}.}
$$

This does not contradict open or closed determinacy: the diagonal payoff has no such regularity requirement.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
