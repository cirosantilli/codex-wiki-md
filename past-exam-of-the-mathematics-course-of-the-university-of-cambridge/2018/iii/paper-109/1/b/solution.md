<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [k-Sperner family](../../../../../../k-sperner-family.md) meets every [maximal chain in a Boolean lattice](../../../../../../maximal-chain-in-a-boolean-lattice.md) in at most $k$ members. The random-chain calculation in part (a) therefore gives the generalized [LYM inequality](../../../../../../lubell-yamamoto-meshalkin-inequality.md) $L(\mathcal A)\leq k$. Define the proportion of rank $i$ that is present by

$$
x_i=\frac{|\mathcal A\cap X^{(i)}|}{\binom ni},\qquad 0\leq x_i\leq1.
$$

Then $\sum_i x_i=L(\mathcal A)\leq k$ and $w(\mathcal A)=\sum_i u(i)x_i$. This reduces the [weighted theorem for k-Sperner families](../../../../../../weighted-theorem-for-k-sperner-families.md) to allocating at most $k$ units of mass among ranks, each of capacity one.

To handle ties explicitly, let $t>0$ be the $k$th largest value among the $u(i)$, let $H=\{i:u(i)>t\}$, and put $h=|H|<k$. Then

$$
\begin{aligned}
w(\mathcal A)&=t\sum_i x_i+\sum_{i\in H}(u(i)-t)x_i-\sum_{u(i)<t}(t-u(i))x_i\\
&\leq tk+\sum_{i\in H}(u(i)-t)\\
&=\sum_{i\in H}u(i)+(k-h)t.
\end{aligned}
$$

The last expression is exactly the sum of the $k$ largest rank weights, with multiplicity. Writing those values in descending order as $u_{(1)},\ldots,u_{(n+1)}$, the answer is

$$
\boxed{w(\mathcal A)\leq\sum_{j=1}^k u_{(j)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
