<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

In a [zero-sum game](../../../../../zero-sum-game.md) with the row player maximizing, a sufficient saddle certificate is that $p,q$ are probability vectors and

$$
Aq\le v\mathbf1,\qquad p^TA\ge v\mathbf1^T.
$$

Every row mixture then gains at most $v$ against $q$, and every column mixture concedes at least $v$ against $p$. Their pairing must equal $v$, proving optimality.

For the [cost-weighted finite search game](../../../../../cost-weighted-finite-search-game.md), order Colin's six columns as $123,132,213,231,312,321$ and Rowena's rows as $1,2,3$. The payoff [matrix](../../../../../matrix.md) is

$$
\boxed{A=\begin{pmatrix}
c_1&c_1&c_1+c_2&c&c_1+c_3&c\\
c_1+c_2&c&c_2&c_2&c&c_2+c_3\\
c&c_1+c_3&c&c_2+c_3&c_3&c_3
\end{pmatrix},\quad c=c_1+c_2+c_3.}
$$

Under the proposed search mixture, an alternative location $i$ precedes the hiding location $j$ with probability $(c_i+c_k/2)/c$, where $k$ is the third location. The expected cost conditional on hiding at $j$ is consequently

$$
c_j+\frac{c_i^2+c_k^2+c_ic_k}{c}
=\frac{c^2+c_1^2+c_2^2+c_3^2}{2c}=:v.
$$

It is independent of $j$, giving the upper bound $\mathrm{value}\le v$.

Choose $p_i=c_i/c$. Against any order $i,j,k$, its expected cost is

$$
\frac{c_i^2+c_j(c_i+c_j)+c_kc}{c}
=\frac{\sum_i c_i^2+\sum_{i<j}c_ic_j}{c}=v.
$$

This gives the matching lower bound. Thus

$$
\boxed{p_i=c_i/c,\qquad q_{ijk}=c_i/(2c),\qquad
\mathrm{value}=\frac{c^2+\sum_i c_i^2}{2c}.}
$$

Both strategies equalize the opponent's pure actions, giving the stated saddle certificate.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
