<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

In a finite two-person [zero-sum game](../../../../../zero-sum-game.md) the row player chooses $i$, the column player chooses $j$, and the row player receives $a_{ij}$ while the column player receives $-a_{ij}$. The row player maximizes that payoff and the column player minimizes it. Mixed strategies are [probability](../../../../../probability.md) [vectors](../../../../../vector.md) $x\in\mathbb R^m$ and $y\in\mathbb R^n$, giving expected row payoff $x^TAy$.

Against a fixed row mixture, the worst column is a pure column, so the row problem introduces its guaranteed payoff $v$:

$$
\boxed{\max_{x,v}v:\quad x\geq0,\quad\mathbf1^Tx=1,\quad A^Tx\geq v\mathbf1.}
$$

Similarly the column player minimizes an upper guarantee $w$:

$$
\boxed{\min_{y,w}w:\quad y\geq0,\quad\mathbf1^Ty=1,\quad Ay\leq w\mathbf1.}
$$

The values $v,w$ are unrestricted real variables; no positivity shift of the [matrix](../../../../../matrix.md) is required.

To see the [linear programming duality](../../../../../linear-programming-duality.md) explicitly, introduce nonnegative multipliers $y$ for the first problem's payoff inequalities and multiplier $w$ for its normalization. Its upper-bound Lagrangian is

$$
\mathcal L=v+y^T(A^Tx-v\mathbf1)+w(1-\mathbf1^Tx)
=w+v(1-\mathbf1^Ty)+x^T(Ay-w\mathbf1).
$$

The supremum over free $v$ and nonnegative $x$ is finite precisely when $\mathbf1^Ty=1$ and $Ay\leq w\mathbf1$, and is then $w$. Minimizing it gives the displayed column problem, proving that the programs are a dual pair.

A sufficient optimality certificate is a pair of [probability](../../../../../probability.md) [vectors](../../../../../vector.md) and a common value $v_*$ satisfying

$$
\boxed{Ay\leq v_*\mathbf1,\qquad A^Tx\geq v_*\mathbf1.}
$$

Equivalently, both programs are feasible with equal values. Positive-probability rows then have $(Ay)_i=v_*$ and positive-probability columns have $(A^Tx)_j=v_*$, the [complementary slackness](../../../../../complementary-slackness.md) conditions. These conditions certify a [saddle point](../../../../../saddle-point.md) and hence optimal mixed strategies for both players.

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
