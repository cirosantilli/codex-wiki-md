<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the game $G(A)$, where $A\subseteq\omega^\omega$, the players alternately choose [natural numbers](../../../../../../natural-number.md) and produce a [sequence](../../../../../../sequence.md) $x$. Player I wins exactly when $x\in A$. A [strategy in an infinite game](../../../../../../strategy-in-an-infinite-game.md) assigns a move to every finite position where its player is to move; it is winning if every play following it is won by that player. A game is determined if one player has a [winning strategy](../../../../../../winning-strategy-in-an-infinite-game.md). Both cannot have [winning strategies](../../../../../../winning-strategy-in-an-infinite-game.md), since their joint play would have to be won by both. The [axiom of determinacy](../../../../../../axiom-of-determinacy.md) asserts

$$
\boxed{\mathsf{AD}:\quad \text{every }G(A),\ A\subseteq\omega^\omega,\ \text{is determined}.}
$$

Without assuming [AD](../../../../../../axiom-of-determinacy.md), one can prove determinacy for finite games by backward induction, and for games with open or closed payoffs by the following argument. Give $\omega^\omega$ its [product topology](../../../../../../product-topology.md) of discrete move coordinates. If $A$ is open, let $W_0$ be the finite positions whose entire cylinder of extensions lies in $A$. Form a [winning-position attractor in an infinite game](../../../../../../winning-position-attractor-in-an-infinite-game.md) by [transfinite recursion](../../../../../../transfinite-recursion.md): add an I-position if some child has already been added, and add an II-position if all its children have already been added. Take [unions](../../../../../../set-union.md) at limits. The process stabilizes because there are only set-many positions and each genuine successor change adds a new one.

An added nonterminal position receives its least entry [ordinal](../../../../../../ordinal.md). At an I-position in the stable attractor, choose a child of smaller rank; at an II-position every child has smaller rank. Thus every play following I's rank-decreasing [strategy](../../../../../../strategy-in-an-infinite-game.md) must reach $W_0$: an infinite strictly descending [sequence](../../../../../../sequence.md) of [ordinals](../../../../../../ordinal.md) cannot exist. The resulting play is in $A$, so I wins from any position in the attractor.

Outside the attractor, every child of an I-position remains outside, and an II-position has some child outside. Otherwise the ranks of all its children would have a set-sized [supremum](../../../../../../supremum.md) and the parent would have been added at a later stage. II chooses such a child and keeps the play outside $W_0$ forever. If its outcome were in the [open set](../../../../../../open-set.md) $A$, some finite prefix would have its entire cylinder in $A$, contrary to this avoidance. Therefore II wins from outside. With natural-number moves the least suitable child may be chosen at each position, so no [choice](../../../../../../axiom-of-choice.md) axiom is needed for these [strategies](../../../../../../strategy-in-an-infinite-game.md). This proves [open determinacy](../../../../../../open-determinacy.md). For a closed payoff, apply the same argument to its open complement with the players' winning roles interchanged. Clopen payoffs are included in both results.

Now assume [AC](../../../../../../axiom-of-choice.md) and construct an undetermined game. The [set](../../../../../../set-split.md) of [strategies](../../../../../../strategy-in-an-infinite-game.md) for either player has [cardinality](../../../../../../cardinality.md) $\mathfrak c=2^{\aleph_0}$, since a [strategy](../../../../../../strategy-in-an-infinite-game.md) is a [function](../../../../../../function-split.md) on a countably infinite [set](../../../../../../set-split.md) of positions. Each fixed [strategy](../../../../../../strategy-in-an-infinite-game.md) is compatible with $\mathfrak c$ plays: the other player's [sequence](../../../../../../sequence.md) of freely chosen moves determines distinct full plays. Use [choice](../../../../../../axiom-of-choice.md) to enumerate I's [strategies](../../../../../../strategy-in-an-infinite-game.md) as $(\sigma_\alpha)_{\alpha<\mathfrak c}$ and II's as $(\tau_\alpha)_{\alpha<\mathfrak c}$, and [well-order](../../../../../../well-order.md) the space of plays.

Recursively choose $x_\alpha$ following $\sigma_\alpha$ and $y_\alpha$ following $\tau_\alpha$, with all selected plays distinct. At stage $\alpha$ fewer than $\mathfrak c$ plays have been used, while each compatible-play [set](../../../../../../set-split.md) has size $\mathfrak c$, so fresh choices exist; take the least ones in the fixed [well-order](../../../../../../well-order.md). This does not require regularity of $\mathfrak c$, since $|\alpha|<\mathfrak c$ for every $\alpha$ below its initial [ordinal](../../../../../../ordinal.md).

Put $A=\{y_\alpha:\alpha<\mathfrak c\}$. Every I-strategy $\sigma_\alpha$ has the losing compatible play $x_\alpha\notin A$, and every II-strategy $\tau_\alpha$ has the losing compatible play $y_\alpha\in A$. Therefore neither player has a [winning strategy](../../../../../../winning-strategy-in-an-infinite-game.md). This [choice diagonalization of an undetermined game](../../../../../../choice-diagonalization-of-an-undetermined-game.md) proves

$$
\boxed{\mathsf{ZF}\vdash\mathsf{AC}\Rightarrow\neg\mathsf{AD}.}
$$

The elementary determinacy proofs above concern specified definable payoff classes; the diagonal construction explains why extending them to every arbitrary [subset](../../../../../../subset.md) of the play space is incompatible with [choice](../../../../../../axiom-of-choice.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
