<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

We prove the [Borel determinacy theorem](../../../../../borel-determinacy-theorem.md) by reducing each Borel game to a [clopen](../../../../../clopen-set.md) game while preserving winning strategies. The construction permits arbitrary set-sized alphabets; no enumeration of the move set is used. Assume $A\neq\varnothing$. For an empty alphabet the game ends at its initial position, with its assigned terminal outcome, and is trivially determined.

Allow intermediate game trees $T$ to have terminal positions with assigned winners. Write $[T]$ for the space of infinite branches, with its prefix-cylinder topology; the payoff $B\subseteq[T]$ governs infinite plays, while the assigned winners govern finite plays. Question 4's attractor proof still gives open and [clopen](../../../../../clopen-set.md) determinacy: include I-winning terminals among the initial targets and make the opposing terminals absorbing losses.

A [covering of an infinite game](../../../../../covering-of-an-infinite-game.md) consists of a new tree $\widetilde T$, a prefix-preserving map $\pi:\widetilde T\to T$ preserving lengths, and a strategy map $\Phi$ for each player. Old terminal outcomes must be inherited. The strategy map is local in depth: choices before depth $n$ depend only on the given strategy before depth $n$. Its essential lifting requirement is that each original play $x$ following $\Phi(\sigma)$ has a lift $\widetilde x$ following $\sigma$ whose projection is $x$, or whose projection is an initial segment of $x$ and which ends with a loss for the player using $\sigma$. Infinite projections are taken by union of prefixes. A $k$-covering is identical to the original tree, terminal assignments and strategy choices through depth $k$.

These conditions transfer winning strategies for every payoff. Indeed, if $\sigma$ wins the covered game with payoff $\pi^{-1}(B)$, a lift of a play following $\Phi(\sigma)$ cannot be an early loss for its player. The lift therefore projects to the whole original play. Infinite membership in $B$ agrees under projection, and an original terminal loss would also be a loss in the [game covering](../../../../../covering-of-an-infinite-game.md). Hence the original play is won. Call a [game covering](../../../../../covering-of-an-infinite-game.md) an [unravelling of a game payoff](../../../../../unravelling-of-a-game-payoff.md) when $\pi^{-1}(B)$ is [clopen](../../../../../clopen-set.md) in $[\widetilde T]$.

We first construct a $k$-covering unravelling any closed $C\subseteq[T]$. Choose an even $m\geq k$ and leave the first $m$ levels unchanged. At a nonterminal position $p$ of length $m$, I's next move will carry auxiliary information. For each legal ordinary move $a$, let $Z$ be the set of first nonterminal positions strictly beyond $p a$ whose infinite continuations miss $C$: $q\in Z$ means $q$ extends $p a$, $[T_q]\cap C=\varnothing$, and no intervening strict extension of $p a$ has this property. These positions are pairwise incomparable. I plays $(a,X)$, where $X\subseteq Z$.

If $p a$ was already terminal, inherit its outcome. Otherwise II has two types of response. On accepting, II plays $(\mathrm{accept},b)$ with $b$ an ordinary legal move, and subsequent moves are ordinary. When a position $q\in Z$ is reached, end the covered game with a win for I if $q\in X$ and for II if $q\notin X$. Other old terminals retain their winners. On challenging, II plays $(\mathrm{challenge},q,b)$ with $q\in X$ and $pab$ an initial segment of $q$; subsequent play is forced along $q$ until reaching it and then proceeds ordinarily in $T_q$. Original terminal outcomes remain in force. Forget the auxiliary data to define $\pi$.

For an infinite accepted play, no exit in $Z$ was reached. Its projection belongs to $C$: if it did not, closedness would give a prefix cylinder disjoint from $C$, and the first such nonterminal extension strictly beyond $p a$ would have ended the play. An infinite challenged play projects through an exit $q$ and therefore misses $C$. Thus, among infinite plays, the inverse image of $C$ is exactly the acceptance branch of this finite protocol. It is [clopen](../../../../../clopen-set.md), decided at depth $m+2$.

Here are both strategy-transfer maps; these are necessary because continuous projection by itself does not preserve determinacy. Given a strategy $\sigma$ for I in the covered tree, follow its ordinary moves while simulating acceptance of its announcement $X$. If an exit $q\notin X$ is reached, continue arbitrarily: that play has an early covered loss for I as a lift. If $q\in X$ is reached, switch to the continuation prescribed by $\sigma$ under the challenge of $q$. This is consistent with the already observed prefix, since the challenged game forced every intermediate move along $q$. If no exit is reached, acceptance itself supplies the full lift. Old terminal plays lift in the same way. This defines $\Phi(\sigma)$ and verifies the lifting requirement for I.

For a covered strategy $\tau$ for II, at the projected position $p a$ define

$$
Y=\{q\in Z:\text{no announcement }X\subseteq Z\text{ makes }\tau\text{ challenge }q\}.
$$

Against announcement $Y$, the strategy must accept: a challenge would have to name an element of $Y$, contradicting its definition. Simulate this acceptance, including its ordinary response $b$. If an exit $q\in Y$ is reached, it is an early covered loss for II, so continue arbitrarily. If an exit $q\notin Y$ is reached, choose an announcement $X_q$ for which $\tau$ challenges $q$, and switch to that simulation. The challenged game's forced prefix agrees with the observed prefix, including the earlier ordinary response $b$, so it supplies a full lift following $\tau$. If no exit is reached, the original acceptance simulation gives the full lift. This defines $\Phi(\tau)$ and verifies lifting for II. Choices of $X_q$ use the [axiom of choice](../../../../../axiom-of-choice.md) on a set of possibilities.

Both maps are local in depth. The sets $Y$ and the chosen $X_q$ use only II's response function at depth $m+1$; later choices use only strategy values at the already reached depth. The switches do not query choices at later levels. On irrelevant histories assign fixed legal moves. Thus this is a genuine $k$-covering. Complementing $C$ changes neither the [game covering](../../../../../covering-of-an-infinite-game.md) nor its lifting property, and complements of [clopen sets](../../../../../clopen-set.md) are [clopen](../../../../../clopen-set.md). This proves the base construction for both closed and open payoff sets.

We next give the limiting construction needed for the induction. Coverings compose by composing their position and strategy maps; lifting successively verifies the same lifting condition. Suppose

$$
\cdots\longrightarrow T_2\longrightarrow T_1\longrightarrow T_0
$$

is a sequence of [game coverings](../../../../../covering-of-an-infinite-game.md) whose $i$th map leaves depth $k+i$ unchanged. For each finite depth $d$, the trees and terminal assignments through that depth eventually stop changing. Define $T_\infty$ using these stabilized levels. Its map to $T_i$ on a position of length $d$ is the composite from any sufficiently late stage; stabilization makes the value independent of the stage. Define strategy maps in the same way, using their locality in depth. These maps respect the tree, terminal outcomes and composition, and leave depth $k$ unchanged.

To check lifting, start with a play of $T_i$ consistent with the projected strategy. Lift the entire play successively through the later [game coverings](../../../../../covering-of-an-infinite-game.md), using the corresponding projected strategy at each stage. If all these lifts are infinite, each projects to the preceding one and each finite prefix eventually stabilizes, giving the desired infinite lift in $T_\infty$. If a premature own-player loss occurs, later lifts have nonincreasing finite lengths, and those lengths and their prefixes eventually stabilize. This gives a terminal own-player loss in $T_\infty$, which is exactly the allowed exceptional lift. The same reasoning handles original finite terminal plays. Thus $T_\infty$ covers every $T_i$. This argument uses level stabilization, not compactness of an infinitely branching tree.

Now induct on the countable [Borel hierarchy](../../../../../borel-hierarchy.md) rank, with the strengthened assertion: for every game tree on any set alphabet and every $k$, a payoff of that rank has a $k$-covering unravelling it. The base case of open or [closed sets](../../../../../closed-set.md) was proved above. Complements preserve the assertion using the same [game covering](../../../../../covering-of-an-infinite-game.md). For the union step, write $B=\bigcup_{n<\omega}B_n$ with constituent sets of smaller rank. Starting at $T_0=T$, successively choose a $(k+n)$-covering $T_{n+1}\to T_n$ that unravels the inverse image of $B_n$ under the composite map to $T$. This is legitimate because continuous inverse images preserve [Borel hierarchy](../../../../../borel-hierarchy.md) rank, and the induction assertion ranges over all trees and alphabets, including the enlarged ones produced by earlier [game coverings](../../../../../covering-of-an-infinite-game.md).

In the stabilized inverse limit, each pulled-back $B_n$ is [clopen](../../../../../clopen-set.md), because the later projection to the stage where it was unravelled is continuous. Their union is therefore open. Apply the already proved open-set unravelling construction once more, with preservation depth $k$, and compose with the limit [game covering](../../../../../covering-of-an-infinite-game.md). The result unravels $B$ itself. This proves the strengthened assertion at every successor or limit countable [Borel hierarchy](../../../../../borel-hierarchy.md) rank. Every Borel set arises at some such rank: countable unions take the supremum of countably many countable ranks and then one further stage, and complements do not leave the generated hierarchy.

Apply the assertion to $T=A^{<\omega}$ and $k=0$. The covered payoff is [clopen](../../../../../clopen-set.md) and hence determined by Question 4, including its assigned finite terminal outcomes. Transfer its winning strategy through the [game covering](../../../../../covering-of-an-infinite-game.md). We obtain

$$
\boxed{B\subseteq A^\omega\text{ Borel}\Longrightarrow\text{one player has a winning strategy in }G(B).}
$$

Every auxiliary alphabet and strategy collection used above is a set. The argument uses power sets and replacement to build those collections and their iterated [game coverings](../../../../../covering-of-an-infinite-game.md), and the axiom of choice for strategy selections; it does not require $A$ to be countable.

## ↑ Ancestors (10)

1. [10](../10.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
