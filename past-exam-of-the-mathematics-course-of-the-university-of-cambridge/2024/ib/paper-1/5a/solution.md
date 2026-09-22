<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

For distinct nodes, define the divided difference by

$$
f[x_0,\ldots,x_k]
=\sum_{j=0}^k
\frac{f(x_j)}{\prod_{\substack{0\leq i\leq k\\i\ne j}}(x_j-x_i)}.
$$

This is the coefficient of $x^k$ in the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) through the first $k+1$ data points.

Let $p_k$ denote that interpolating [polynomial](../../../../../polynomial-split.md). The difference $p_k-p_{k-1}$ vanishes at $x_0,\ldots,x_{k-1}$, so

$$
p_k(x)-p_{k-1}(x)=c_k\prod_{i=0}^{k-1}(x-x_i).
$$

The Lagrange formula shows that the leading coefficient of $p_k$ is $f[x_0,\ldots,x_k]$, whereas $p_{k-1}$ has degree at most $k-1$. Hence $c_k=f[x_0,\ldots,x_k]$. Starting with $p_0=f(x_0)$ and iterating gives the [Newton interpolation polynomial](../../../../../newton-polynomial.md)

$$
\boxed{
p_n(x)=f(x_0)+\sum_{k=1}^n f[x_0,\ldots,x_k]
\prod_{i=0}^{k-1}(x-x_i)}.
$$

The divided-difference recurrence is

$$
\boxed{
f[x_0,\ldots,x_k]
=\frac{f[x_1,\ldots,x_k]-f[x_0,\ldots,x_{k-1}]}
{x_k-x_0}}.
$$

For three nodes, the triangular table is

$$
\begin{array}{ccc}
f[x_0]&\longrightarrow&f[x_0,x_1]\longrightarrow f[x_0,x_1,x_2]\\
f[x_1]&\longrightarrow&f[x_1,x_2]\\
f[x_2]
\end{array}
$$

where each entry in a new column uses the two adjacent entries to its left. There are $n$ first differences, $n-1$ second differences, and so on, each requiring one division. The exact total is

$$
\boxed{n+(n-1)+\cdots+1=\frac{n(n+1)}2}.
$$

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
