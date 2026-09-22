<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

Let $p\in\mathbb R^m$ be Player I's row-strategy distribution and let $e$ denote an all-ones vector of the required dimension. Against column $j$, the expected payoff is $(p^TA)_j$. Thus Player I's [matrix-game optimization problem](../../../../../matrix-game-optimization-problem.md) is

$$
\boxed{
\max_{p,v}v
\quad\text{subject to}\quad
A^Tp\geq ve,quad e^Tp=1,quad p\geq0}.
$$

Equivalently, Player I maximizes $\min_j(p^TA)_j$ over the probability simplex.

Let $q^*$ be an optimal mixed strategy for Player II and let the game value be $v^*$. A sufficient condition for a probability vector $p$ to be optimal for Player I is

$$
\boxed{p^TA\geq v^*e^T}.
$$

Indeed, this makes $p$ guarantee at least $v^*$ against every pure column and hence every mixed strategy. On the other hand, the optimality of $q^*$ prevents any row strategy from obtaining more than $v^*$ against $q^*$. Therefore $p$ is optimal. This is the [mixed-strategy optimality certificate for a matrix game](../../../../../mixed-strategy-optimality-certificate-for-a-matrix-game.md).

Now suppose that $A$ is invertible and symmetric and that $A^{-1}e\geq0$. Put

$$
c=e^TA^{-1}e,
\qquad
p=q=\frac{A^{-1}e}{c}.
$$

The vector $A^{-1}e$ is nonzero and nonnegative, so $c>0$ and $p,q$ are probability vectors. Since $A$ is symmetric,

$$
p^TA=\frac{e^T}{c},
\qquad
Aq=\frac e c.
$$

Thus $p$ guarantees $1/c$ and $q$ holds the payoff to $1/c$. By the [minimax theorem](../../../../../minimax-theorem.md),

$$
\boxed{v^*=\frac1{e^TA^{-1}e}}.
$$

This proves the [symmetric inverse formula for a matrix-game equilibrium](../../../../../symmetric-inverse-formula-for-a-matrix-game-equilibrium.md).

For the card game, the payoff matrix to Player I is

$$
A=\begin{pmatrix}
2&3&4\\
3&4&-5\\
4&-5&-6
\end{pmatrix}.
$$

It is symmetric and invertible, and direct solution of $Ax=e$ gives

$$
A^{-1}e=\frac1{114}
\begin{pmatrix}41\\4\\5\end{pmatrix},
\qquad
e^TA^{-1}e=\frac{25}{57}.
$$

The preceding result therefore gives the same optimal strategy for both players:

$$
\boxed{
p^*=q^*=\begin{pmatrix}
41/50\\[2pt]2/25\\[2pt]1/10
\end{pmatrix}}.
$$

Thus each player chooses cards $1,2,3$ with probabilities $41/50,2/25,1/10$, respectively, and the value to Player I is

$$
\boxed{v^*=\frac{57}{25}\text{ pounds}}.
$$

This is the [three-card threshold-sum zero-sum game](../../../../../three-card-threshold-sum-zero-sum-game.md).

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
