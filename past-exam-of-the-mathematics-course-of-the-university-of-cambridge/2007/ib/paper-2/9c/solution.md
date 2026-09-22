<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The row player maximizes the payoff and the column player minimizes it. Row three is weakly dominated by row one, so the row player can discard it. On the remaining two rows, column two is weakly dominated by column three, so the column player can discard column two. The reduced [zero-sum game](../../../../../zero-sum-game.md) has payoff matrix

$$
\begin{pmatrix}2&4\\3&2\end{pmatrix}.
$$

If the first row is chosen with probability $r$, the expected payoffs against its two columns are $3-r$ and $2+2r$. Equalizing them gives $r=1/3$ and value $8/3$. If the first column is chosen with probability $s$, the payoffs of the two rows are $4-2s$ and $2+s$. Equalizing them gives $s=2/3$.

Restoring the original indexing, the optimal [mixed strategies](../../../../../mixed-strategy.md) and [value of a zero-sum game](../../../../../value-of-a-zero-sum-game.md) are

$$
\boxed{\mathbf r=(1/3,2/3,0),\qquad
\mathbf s=(2/3,0,1/3),\qquad v=8/3.}
$$

To verify these against every original strategy, the row mixture gives the three column payoffs $(8/3,3,8/3)$, each at least $v$. The column mixture gives the three row payoffs $(8/3,8/3,7/3)$, each at most $v$. Thus each [mixed strategy](../../../../../mixed-strategy.md) guarantees the stated value, including against the discarded strategies. The strict inequalities for column two and row three also force those probabilities to be zero in any optimal strategy, and the remaining equalities determine the displayed mixtures uniquely.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
