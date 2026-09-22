<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

Let $p$ be the row player's [mixed strategy](../../../../../mixed-strategy.md) and $q$ the column player's [mixed strategy](../../../../../mixed-strategy.md). The fourth row is strictly dominated by the first. A useful candidate mixes the first two rows so that their first and third column payoffs agree. If the first row has probability $t$, these payoffs are $7t-2$ and $2-7t$, giving $t=2/7$ and common value zero.

To prove that these are [optimal mixed strategies](../../../../../optimal-mixed-strategy.md), use the two explicit [mixed strategies](../../../../../mixed-strategy.md)

$$
\boxed{p=(2/7,5/7,0,0)^T,\qquad q=(1/2,0,1/2)^T,\qquad v=0.}
$$

Their payoff vectors satisfy

$$
p^TA=(0,11/7,0),\qquad Aq=(0,0,-1/2,-1)^T.
$$

Thus the row player guarantees a payoff at least zero against every column [mixed strategy](../../../../../mixed-strategy.md), and the column player guarantees a payoff at most zero against every row [mixed strategy](../../../../../mixed-strategy.md). This matching pair proves that **the value of the zero-sum game is zero**.

These [optimal mixed strategies](../../../../../optimal-mixed-strategy.md) are also unique. Since $Aq$ is strictly negative in rows three and four, any optimal row strategy gives them probability zero. Against columns one and three it must then satisfy both $7t-2\geq0$ and $2-7t\geq0$, so $t=2/7$. Similarly, $p^TA$ is strictly positive in column two, forcing an optimal column strategy to avoid that column; its constraints against rows one and two then force equal weights on columns one and three.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
