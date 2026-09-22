<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In an [infinite game of perfect information](../../../../../infinite-game-of-perfect-information.md), the players alternately choose elements of a nonempty set $A$, producing $x\in A^\omega$. Player I wins when $x$ belongs to the payoff set $B$. A [strategy in an infinite game](../../../../../strategy-in-an-infinite-game.md) chooses a move at each position where its player moves, and a [winning strategy in an infinite game](../../../../../winning-strategy-in-an-infinite-game.md) wins against every possible opposing play. The [Gale-Stewart theorem](../../../../../open-determinacy.md) states that such a game is determined when $B$ is open in the [product topology](../../../../../product-topology.md) of discrete $A$. The same holds for closed payoff sets and, more strongly, for every $G_\delta$ payoff set.

For [open determinacy](../../../../../open-determinacy.md), let $P=A^{<\omega}$ be the positions and $D=\{s:[s]\subseteq B\}$ the prefixes certifying a win for I, where $[s]$ is the extension [cylinder set](../../../../../cylinder-set.md). Form the [winning-position attractor in an infinite game](../../../../../winning-position-attractor-in-an-infinite-game.md) by [transfinite recursion](../../../../../transfinite-recursion.md): start at $W_0=D$, at a successor stage add I-positions with some successor already in $W_\alpha$ and II-positions with all successors in $W_\alpha$, and take unions at limits. This increasing sequence stabilizes, since its positions form a set. Call the stable set $W$.

Each position in $W\setminus D$ has a least entry [ordinal](../../../../../ordinal.md), necessarily a successor. I chooses a successor with smaller entry [ordinal](../../../../../ordinal.md); every II successor has smaller entry [ordinal](../../../../../ordinal.md). An infinite strictly decreasing sequence of [ordinals](../../../../../ordinal.md) is impossible, so play reaches $D$ in finitely many moves. This gives I a [winning strategy in an infinite game](../../../../../winning-strategy-in-an-infinite-game.md) from every position in $W$. Outside $W$, all I moves stay outside, while II can choose a move outside. The [axiom of choice](../../../../../axiom-of-choice.md) selects those moves simultaneously. Such a play never reaches $D$, so it is outside the open payoff set. Thus II wins from the complement of $W$, proving determinacy. Interchanging the players and complementing the payoff gives closed determinacy.

We prove the $G_\delta$ strengthening via [Buchi games](../../../../../buchi-game.md), including their determinacy argument. On a set of positions $S$ with nonempty successor sets, put

$$
\operatorname{Pre}(X)=\{s\text{ at I's turn}:\exists\text{ successor in }X\}\cup\{s\text{ at II's turn}:\text{every successor is in }X\}.
$$

For a specified set $F$ of marked positions, I's objective is to visit $F$ infinitely often. For each $X\subseteq S$, let $H(X)$ be the least fixed point obtained by starting $Y_0=\varnothing$ and iterating

$$
Y\longmapsto(F\cap\operatorname{Pre}(X))\cup\operatorname{Pre}(Y)
$$

with unions at limits. Its inner entry ranks let I force a visit to $F\cap\operatorname{Pre}(X)$. The operation $H$ is monotone. Starting at $X_0=S$, iterate $X_{\alpha+1}=H(X_\alpha)$ with intersections at limits. This descending sequence stabilizes at $W=H(W)$.

From $W$, the inner ranks force a marked position with a next move still in $W$. I chooses such a move, and the construction repeats. At II-positions all necessary moves stay in the indicated inner attractor, or in $W$ at a marked position. Every round takes finitely many moves by decreasing inner ranks. I therefore forces infinitely many marked visits.

For $s\notin W$, let $\alpha$ be its removal rank: $s\in X_\alpha\setminus X_{\alpha+1}$. Since $s\notin H(X_\alpha)$, at I's turn all successors lie outside $H(X_\alpha)$, and at II's turn there is a successor outside it. II chooses such successors. If also $s\in F$, then $s\notin\operatorname{Pre}(X_\alpha)$; II can choose outside $X_\alpha$, or every I move lies outside $X_\alpha$. Along this strategy removal ranks never increase and strictly decrease after each marked visit. Infinitely many visits would give an infinite [ordinal](../../../../../ordinal.md) descent, so II wins. This proves [Buchi game](../../../../../buchi-game.md) determinacy on a set-sized arena without any countability restriction.

Now write the original payoff as $B=\bigcap_{n<\omega}U_n$, with each $U_n$ open. Add a deterministic monitor to the finite position, initially $n=0$. At each new prefix, if its cylinder is contained in $U_n$, increment the monitor and mark that step. For a play $x$, the monitor increments infinitely often exactly when $x\in B$. In one direction every increment certifies the next required open set. In the other, after the monitor reaches $n$, openness of $U_n$ supplies a later certifying prefix, so it eventually reaches $n+1$. The expanded game is a [Buchi game](../../../../../buchi-game.md); its monitor is determined by the observed finite play, so its winning strategy transfers directly to the original game. Consequently

$$
\boxed{B\in G_\delta\Longrightarrow G(B)\text{ is determined}.}
$$

Complementing and interchanging players also gives determinacy for $F_\sigma$ payoff sets. These arguments work on pruned game subtrees as well, and assigned terminal winners can be incorporated by replacing each terminal position by an absorbing position with the corresponding outcome.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
