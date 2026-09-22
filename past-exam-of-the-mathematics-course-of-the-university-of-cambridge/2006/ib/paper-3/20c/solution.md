<h1 id="20c/solution">Solution</h1>

↑ **Parent:** [20C](../20c.md)

In a [zero-sum game](../../../../../zero-sum-game.md), an entry $a_{ij}$ is the net amount received by the row player when the players choose actions $i,j$; the column player receives its negative. A [mixed strategy](../../../../../mixed-strategy.md) $p$ has nonnegative entries summing to one. Against column strategy $q$, expected row payoff is $p^TAq$. An optimal row strategy maximizes its guaranteed payoff $\min_qp^TAq$; an optimal column strategy minimizes $\max_pp^TAq$.

The betting payoff must subtract the player's own stake: a winner receives both stakes but has already paid its own. Its net gain is the opponent's stake, and a loser loses its own. Ties give zero. Thus the row-payoff [matrix](../../../../../matrix.md) is

$$
\boxed{A=\begin{pmatrix}
0&-1&-1&4\\
1&0&-2&-2\\
1&2&0&-3\\
-4&2&3&0
\end{pmatrix}.}
$$

It is antisymmetric. Interchanging players therefore changes the sign of the game value while leaving the game unchanged, so its value is zero. An optimal column strategy $p$ must prevent any pure row choice from gaining positively, namely $(Ap)_i\le0$. Antisymmetry then also gives $p^TA\ge0$, so the same vector is an optimal row strategy. This is the [support certificate for an antisymmetric matrix game](../../../../../support-certificate-for-an-antisymmetric-matrix-game.md).

Seek a mixture supported on actions $1,3,4$ making those three opposing choices indifferent. Their zero-payoff equations are

$$
-p_3+4p_4=0,\qquad p_1-3p_4=0,\qquad -4p_1+3p_3=0.
$$

With $p_1+p_3+p_4=1$, these give

$$
\boxed{p=\begin{pmatrix}3/8\\0\\1/2\\1/8\end{pmatrix}.}
$$

Check every opponent action, including the omitted second one:

$$
Ap=\begin{pmatrix}0\\-7/8\\0\\0\end{pmatrix}\le0.
$$

This verifies optimality rather than simply assuming that a support choice is valid.

It is also unique. Let $r$ be any other optimal strategy, so $Ar\le0$. For the displayed $p$, antisymmetry gives $p^TAr=-(Ap)^Tr=(7/8)r_2$. The left side is nonpositive and the right side nonnegative, forcing $r_2=0$. Since the other three entries of $p$ are positive, $p^TAr=0$ also forces $(Ar)_1=(Ar)_3=(Ar)_4=0$. Their equations and normalization recover the same probabilities. Thus **both players' unique optimal strategy uses bets one, three and four in the proportions $3:4:1$**.

## ↑ Ancestors (10)

1. [20C](../20c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
