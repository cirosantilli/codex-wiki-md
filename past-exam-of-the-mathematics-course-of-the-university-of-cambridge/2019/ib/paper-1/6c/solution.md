<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

For distinct [interpolation nodes](../../../../../interpolation-node.md) $x_0,\ldots,x_m$, define the degree-$m$ [divided difference](../../../../../divided-difference.md) by

$$
f[x_0,\ldots,x_m]
=\sum_{j=0}^m\frac{f(x_j)}{\prod_{\substack{0\leq k\leq m\\k\ne j}}(x_j-x_k)}.
$$

It is the leading coefficient of the unique degree-at-most-$m$ [interpolating polynomial](../../../../../polynomial-interpolation.md) through those data.

Define

$$
p_n(x)=f[x_0]+\sum_{m=1}^nf[x_0,\ldots,x_m]\prod_{i=0}^{m-1}(x-x_i).
$$

The partial polynomial $p_m$ agrees with $p_{m-1}$ at $x_0,\ldots,x_{m-1}$. Moreover, the explicit formula for the divided difference gives

$$
f[x_0,\ldots,x_m]
=\frac{f(x_m)-p_{m-1}(x_m)}{\prod_{i=0}^{m-1}(x_m-x_i)},
$$

so $p_m(x_m)=f(x_m)$. Induction shows that $p_n(x_j)=f(x_j)$ for every $j$. By uniqueness of [polynomial interpolation](../../../../../polynomial-interpolation.md), this is the required [Newton interpolation polynomial](../../../../../newton-polynomial.md).

For the recursion, substitute the explicit formulas for $f[x_1,\ldots,x_m]$ and $f[x_0,\ldots,x_{m-1}]$. For an interior index $j$, the coefficient of $f(x_j)$ in their difference is

$$
\frac1{(x_j-x_m)\prod_{\substack{1\leq k\leq m-1\\k\ne j}}(x_j-x_k)}
-\frac1{(x_j-x_0)\prod_{\substack{1\leq k\leq m-1\\k\ne j}}(x_j-x_k)}
=\frac{x_m-x_0}{\prod_{\substack{0\leq k\leq m\\k\ne j}}(x_j-x_k)}.
$$

The endpoint terms satisfy the same identity directly. Dividing by $x_m-x_0$ therefore gives

$$
\boxed{f[x_0,\ldots,x_m]
=\frac{f[x_1,\ldots,x_m]-f[x_0,\ldots,x_{m-1}]}{x_m-x_0}}.
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
