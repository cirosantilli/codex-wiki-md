<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

In a two-player [zero-sum game](../../../../../zero-sum-game.md), entry $a_{ij}$ is player I's gain, and player II's loss, when pure strategies $i,j$ are chosen. Player I maximizes the expected payoff, player II minimizes it. A [mixed strategy](../../../../../mixed-strategy.md) is a probability vector. Sufficient optimality conditions for $p,q$ and value $v$ are

$$
p\ge0,\quad q\ge0,\quad \mathbf1^Tp=\mathbf1^Tq=1,\qquad
Aq\le v\mathbf1,\quad p^TA\ge v\mathbf1^T.
$$

Indeed $q$ keeps every opposing payoff at most $v$, while $p$ guarantees at least $v$ against every opposing [mixed strategy](../../../../../mixed-strategy.md); their joint payoff must equal $v$.

A pure strategy for the informed player specifies one action after each possible outcome. Order these contingent choices as $(P,P),(P,B),(B,P),(B,B)$, with the first action for a head. The columns are fold and call. Averaging over the fair coin gives the payoff [matrix](../../../../../matrix.md), in currency units,

$$
A=\begin{pmatrix}-1&-1\\0&-3/2\\0&1/2\\1&0\end{pmatrix}.
$$

For example, row $(B,P)$ against call averages a gain of two and a loss of one, giving $1/2$.

Take

$$
\boxed{p=(0,0,2/3,1/3)^T,\qquad q=(1/3,2/3)^T.}
$$

Then $Aq=(-1,-1,1/3,1/3)^T$ and $p^TA=(1/3,1/3)$, so the sufficient inequalities hold with **game value $v=1/3$ to player I**. In behavioral terms, I always bets on a head and bets with probability $1/3$ on a tail; II calls with probability $2/3$. The four rows describe complete contingent plans, not four coin outcomes.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
