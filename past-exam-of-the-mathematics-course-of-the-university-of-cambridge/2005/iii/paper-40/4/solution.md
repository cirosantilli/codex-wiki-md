<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $v:2^N\to\mathbb R$, $v(\varnothing)=0$, be a [coalitional game](../../../../../transferable-utility-game.md) with $n=|N|$. The [Shapley value](../../../../../shapley-value.md) is

$$
\phi_i(N,v)=\sum_{S\subseteq N\setminus\{i\}}
\frac{|S|!(n-|S|-1)!}{n!}\bigl(v(S\cup\{i\})-v(S)\bigr).
$$

Equivalently, choose a uniformly random player ordering and average each player's [marginal contribution](../../../../../marginal-contribution.md) when that player joins its predecessors. The coefficient counts precisely the orderings with predecessor set $S$.

The standard axioms are efficiency, $\sum_i\phi_i=v(N)$; symmetry, giving equal values to players with identical [marginal contributions](../../../../../marginal-contribution.md); the dummy-player property, giving $\phi_i=v(\{i\})$ if every [marginal contribution](../../../../../marginal-contribution.md) of $i$ equals $v(\{i\})$; and additivity, $\phi_i(v+w)=\phi_i(v)+\phi_i(w)$. The null-player form of the dummy axiom gives zero to a player contributing nothing. These properties characterize the [Shapley value](../../../../../shapley-value.md). They also follow directly from its formula: efficiency telescopes along each ordering, symmetry relabels orderings, constant dummy contributions average to themselves, and the sum is linear in $v$.

For [balanced contributions of Shapley values](../../../../../balanced-contributions-of-shapley-values.md), remove player $j$ from a uniformly random ordering. The resulting ordering of $N\setminus\{j\}$ is uniform, so it computes $i$'s [Shapley value](../../../../../shapley-value.md) in the restricted game. If $j$ comes after $i$, removing it does not change $i$'s [marginal contribution](../../../../../marginal-contribution.md). If $j$ precedes $i$, and $S$ consists of $i$'s other predecessors, the difference is

$$
\Delta_{ij}v(S)=v(S\cup\{i,j\})-v(S\cup\{j\})-v(S\cup\{i\})+v(S).
$$

There are $(|S|+1)!(n-|S|-2)!$ full orderings with exactly $S\cup\{j\}$ before $i$. Consequently

$$
\phi_i(N,v)-\phi_i(N\setminus\{j\},v)
=\sum_{S\subseteq N\setminus\{i,j\}}
\frac{(|S|+1)!(n-|S|-2)!}{n!}\Delta_{ij}v(S).
$$

Both the summand and coefficient are unchanged when $i,j$ are interchanged. Thus

$$
\boxed{\phi_i(N,v)-\phi_i(N\setminus\{j\},v)
=\phi_j(N,v)-\phi_j(N\setminus\{i\},v)}.
$$

The restriction keeps all [coalition](../../../../../coalition-game-theory.md) values for the remaining players, exactly matching the payoff comparison after a departure. The identity does not require the differences to be positive.

Now consider the [coverage coalitional game](../../../../../coverage-coalitional-game.md) formed by the finite book sets. For disjoint [coalitions](../../../../../coalition-game-theory.md) $S,T$, put $B(S)=\bigcup_{i\in S}B_i$. Then

$$
v(S\cup T)=v(S)+v(T)-|B(S)\cap B(T)|\leq v(S)+v(T).
$$

Thus coverage is generally subadditive. It is a [superadditive coalitional game](../../../../../superadditive-coalitional-game.md) precisely when the book sets are pairwise disjoint: disjointness makes the displayed formula additive, while a common book of players $i,j$ gives $v(\{i,j\})<v(\{i\})+v(\{j\})$. For example, $B_1=B_2=\{b\}$ gives values $1,1,1$ and disproves unconditional superadditivity. The printed clause must therefore have its disjointness condition apply to superadditivity as well as to [core](../../../../../core-game-theory.md) nonemptiness.

For the [core of a coverage game](../../../../../core-of-a-coverage-game.md), an allocation must satisfy efficiency $\sum_i x_i=v(N)$ and $\sum_{i\in S}x_i\geq v(S)$ for every [coalition](../../../../../coalition-game-theory.md). In particular $x_i\geq|B_i|$. Summing gives

$$
\left|\bigcup_iB_i\right|=\sum_ix_i\geq\sum_i|B_i|.
$$

The reverse inequality always holds, with equality exactly when no book appears in two sets. Therefore overlap makes the [core](../../../../../core-game-theory.md) empty. If the sets are disjoint, $x_i=|B_i|$ gives every [coalition](../../../../../coalition-game-theory.md) exactly its value and is a [core](../../../../../core-game-theory.md) allocation; the singleton lower bounds and efficiency make it the only one. Hence **superadditivity and a nonempty core each occur exactly in the pairwise-disjoint case**.

Finally write the game as a sum over individual books. For a book $b$, let $K_b=\{k:b\in B_k\}$. Its contribution to [coalition](../../../../../coalition-game-theory.md) value is one if the [coalition](../../../../../coalition-game-theory.md) meets $K_b$, and zero otherwise. In a random ordering, player $i$ contributes this book precisely when $i\in K_b$ and is earliest among its $|K_b|$ knowers. Each knower is equally likely to be earliest. Additivity of the [Shapley value](../../../../../shapley-value.md) therefore gives the [Shapley value of a coverage game](../../../../../shapley-value-of-a-coverage-game.md)

$$
\boxed{\phi_i(v)=\sum_{b\in B_i}\frac1{|K_b|}}.
$$

This formula remains valid when books overlap and the [core](../../../../../core-game-theory.md) is empty.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
