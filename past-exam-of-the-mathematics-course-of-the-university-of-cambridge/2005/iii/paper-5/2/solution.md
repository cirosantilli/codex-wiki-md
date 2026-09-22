<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Read equality of the two positive [series](../../../../../series-mathematics.md) as equality of a finite total $M$, so the sequences are summable. This is the [majorization of summable sequences](../../../../../majorization-of-summable-sequences.md) setting. If equality is instead allowed to mean $\infty=\infty$, the assertion is false: the strictly decreasing sequences $x_i=1+1/(i+1)$ and $y_i=2+1/(i+1)$ satisfy every partial-sum inequality and have divergent equal extended totals. But a normalized nonnegative row of any [doubly stochastic matrix](../../../../../doubly-stochastic-matrix.md) averages numbers all at least $2$, and cannot give $x_i<2$. We prove the intended finite-total assertion constructively.

Since $y_j\to0$ and $0<x_1\leq y_1$, there is a finite $k$ such that $y_k\geq x_1>y_{k+1}$. Put

$$
t=\frac{x_1-y_{k+1}}{y_k-y_{k+1}}\in(0,1],
\qquad u=y_k+y_{k+1}-x_1.
$$

The [two-coordinate stochastic averaging](../../../../../two-coordinate-stochastic-averaging.md) [matrix](../../../../../matrix.md) sends $(y_k,y_{k+1})$ to $(x_1,u)$. Move the first of these values to the front by a finite [permutation](../../../../../permutation.md), leaving the other values in decreasing order. The tail is

$$
z=(y_1,\ldots,y_{k-1},u,y_{k+2},y_{k+3},\ldots),
$$

which is decreasing and strictly positive because $y_{k+1}\leq u\leq y_k$.

We need the residual [majorization](../../../../../majorization.md) in order to repeat the construction. For $n<k$, the first $n$ values of $z$ are at least $x_1$, while every target-tail value is at most $x_1$. Thus

$$
\sum_{j=1}^n z_j\geq nx_1\geq\sum_{i=2}^{n+1}x_i.
$$

For $n\geq k$, the residual initial sum is the old initial sum with $x_1$ removed:

$$
\sum_{j=1}^nz_j=\sum_{j=1}^{n+1}y_j-x_1
\geq\sum_{i=2}^{n+1}x_i.
$$

The tail totals also agree, both equalling $M-x_1$. Therefore the same step applies to $(x_2,x_3,\ldots)$ and $z$.

Iterating, let $P^{(m)}$ be the product of the first $m$ finite [permutations](../../../../../permutation.md) and embedded averaging [matrices](../../../../../matrix.md). Each $P^{(m)}$ is a [doubly stochastic matrix](../../../../../doubly-stochastic-matrix.md), each row is a [finitely supported sequence](../../../../../finitely-supported-sequence.md), and the first $m$ entries of $P^{(m)}y$ are $x_1,\ldots,x_m$. Later operations act only on tail rows, so row $i$ becomes permanently fixed once $m\geq i$. Define $p_{ij}$ to be that stabilized row. Then

$$
p_{ij}\geq0,\qquad \sum_jp_{ij}=1,\qquad
x_i=\sum_jp_{ij}y_j.
$$

For every fixed column $j$ and every $m$, its first $m$ stabilized entries sum to at most one, since they are entries of column $j$ in $P^{(m)}$. Consequently $s_j=\sum_i p_{ij}\leq1$. By [Tonelli's theorem](../../../../../tonelli-theorem.md),

$$
M=\sum_i x_i=\sum_j y_j s_j,\qquad
0=\sum_j y_j(1-s_j).
$$

All $y_j$ are strictly positive and every summand in the last expression is nonnegative, so $s_j=1$ for every $j$. Thus **both the row sums and the column sums are one**, and

$$
\boxed{x=Py\quad\text{with }P\text{ doubly stochastic}.}
$$

The finite-total argument is what prevents loss of column mass in the infinite construction. This completes the [doubly stochastic realization of summable-sequence majorization](../../../../../doubly-stochastic-realization-of-summable-sequence-majorization.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
