<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The game is degenerate in the [nondegeneracy of a bimatrix game](../../../../../../nondegeneracy-of-a-bimatrix-game.md) sense. Against the first player's [pure strategy](../../../../../../pure-strategy.md) $4$, the second player's choices $1$ and $2$ are both [best responses](../../../../../../best-response.md), with payoff four. A [mixed strategy](../../../../../../mixed-strategy.md) of support size one therefore has two pure [best responses](../../../../../../best-response.md). The usual [Lemke-Howson algorithm](../../../../../../lemke-howson-algorithm.md) path needs additional tie handling or perturbation in such a game; the [zero-sum game](../../../../../../zero-sum-game.md) structure gives a simpler direct [linear program](../../../../../../linear-programming.md).

Add five to every entry of the first player's matrix, obtaining

$$
B=\begin{pmatrix}5&7&4\\6&5&3\\1&1&5\end{pmatrix}.
$$

This does not change either player's [best responses](../../../../../../best-response.md) or [Nash equilibria](../../../../../../nash-equilibrium.md); it raises the game value by five. Since all entries are positive, its value $v_B$ is positive. If $p$ is a row [mixed strategy](../../../../../../mixed-strategy.md) guaranteeing $v_B$, put $x=p/v_B$. Then $B^Tx\ge\mathbf1$ and $\mathbf1^Tx=1/v_B$.

Conversely any feasible $x$ has $s=\mathbf1^Tx>0$, and $p=x/s$ guarantees payoff $1/s$ in the shifted game. Maximizing that guaranteed payoff is therefore equivalent to minimizing $s$ under $B^Tx\ge\mathbf1$, $x\ge0$. These are precisely the displayed constraints. The dual program maximizes $\mathbf1^Ty$ subject to $By\le\mathbf1$, $y\ge0$; normalizing an optimal $y$ gives the column strategy. This is [positive-payoff linear programming for a matrix game](../../../../../../positive-payoff-linear-programming-for-a-matrix-game.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
