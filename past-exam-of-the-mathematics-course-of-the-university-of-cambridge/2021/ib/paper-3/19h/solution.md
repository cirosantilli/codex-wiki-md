<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

An $m\times n$ [matrix game](../../../../../matrix-game.md) with payoff matrix $A$ is a two-player [zero-sum game](../../../../../zero-sum-game.md): player I chooses a row and receives $A_{ij}$, while player II chooses a column and loses the same amount. For [mixed strategies](../../../../../mixed-strategy.md) $p$ and $q$, the expected payoff to player I is

$$
p^TAq.
$$

Player I's [optimal mixed strategy](../../../../../optimal-mixed-strategy.md) maximizes the payoff guaranteed against every $q$, while player II's minimizes the largest payoff obtainable by any $p$. Thus

$$
\max_p\min_qp^TAq
=v
=\min_q\max_pp^TAq
$$

by the [minimax theorem](../../../../../minimax-theorem.md). Equivalently, optimal strategies satisfy

$$
p^TA\geq v\mathbf1^T,
\qquad
Aq\leq v\mathbf1.
$$

Here $A^T=-A$, so this is an [antisymmetric zero-sum game](../../../../../antisymmetric-zero-sum-game.md). For every probability vector $r$,

$$
r^TAr=0.
$$

It follows that the row player's guaranteed payoff cannot exceed zero and the column player's worst loss cannot be below zero. Minimax therefore gives

$$
\boxed{v=0}.
$$

If $p$ is optimal for player I, then

$$
p^TA\geq0.
$$

Transposing and using $A^T=-A$ gives

$$
Ap\leq0,
$$

which is precisely the optimality condition for player II. Thus every optimal strategy for player I is also optimal for player II.

The condition $Ap\leq0$ explicitly reads

$$
\begin{aligned}
p_2+p_3-4p_4&\leq0,\\
-p_1+2p_3+2p_4&\leq0,\\
-p_1-2p_2+3p_4&\leq0,\\
4p_1-2p_2-3p_3&\leq0.
\end{aligned}
$$

The probability vector

$$
\boxed{p=\frac17(2,4,0,1)^T}
$$

satisfies

$$
Ap=(0,0,-1,0)^T\leq0,
$$

so it is optimal for both players.

To prove uniqueness, let $q$ be any optimal strategy. Since $p$ is optimal for player II and $q$ is optimal for player I,

$$
0\leq q^TAp=-q_3,
$$

and hence $q_3=0$. Writing $q=(a,b,0,d)^T$, the first, second, and fourth inequalities in $Aq\leq0$ give

$$
b\leq4d,\qquad a\geq2d,\qquad b\geq2a.
$$

Consequently

$$
4d\geq b\geq2a\geq4d,
$$

so equality holds throughout: $a=2d$ and $b=4d$. The normalization $a+b+d=1$ yields $d=1/7$. Therefore the displayed $p$ is the unique optimal strategy.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
