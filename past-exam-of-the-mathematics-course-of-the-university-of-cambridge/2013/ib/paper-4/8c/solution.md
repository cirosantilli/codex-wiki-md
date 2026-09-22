<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For distinct nodes, define the [divided difference](../../../../../divided-difference.md) recursively by

$$
f[x_0]=f(x_0),\qquad f[x_0,\ldots,x_k]=\frac{f[x_1,\ldots,x_k]-f[x_0,\ldots,x_{k-1}]}{x_k-x_0}.
$$

Only the function values at the nodes are needed. Induction in this recursion gives

$$
f[x_0,\ldots,x_k]=\sum_{j=0}^k\frac{f(x_j)}{\prod_{0\le i\le k,\ i\ne j}(x_j-x_i)}.
$$

For an interior index $j$, the two terms in the recursive numerator combine using $(x_j-x_0)-(x_j-x_k)=x_k-x_0$; the endpoint terms give the same displayed denominators. This proves the formula, including its symmetry in the nodes.

The [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) on the first $k+1$ nodes is

$$
p_k(x)=\sum_{j=0}^k f(x_j)\frac{\prod_{i\ne j}(x-x_i)}{\prod_{i\ne j}(x_j-x_i)}.
$$

Its leading coefficient is therefore $f[x_0,\ldots,x_k]$. Meanwhile $p_k-p_{k-1}$ vanishes at $x_0,\ldots,x_{k-1}$ and has degree at most $k$. The [factor theorem](../../../../../factor-theorem.md) and the leading coefficient imply

$$
p_k-p_{k-1}=f[x_0,\ldots,x_k]\prod_{i=0}^{k-1}(x-x_i).
$$

Starting from $p_0=f(x_0)$ and summing these identities proves the [Newton interpolation polynomial](../../../../../newton-polynomial.md) formula

$$
\boxed{p_n(x)=f(x_0)+\sum_{k=1}^n f[x_0,\ldots,x_k]\prod_{i=0}^{k-1}(x-x_i).}
$$

The same [factor theorem](../../../../../factor-theorem.md) proves uniqueness: the difference of two interpolants of degree at most $n$ has $n+1$ distinct zeros and must vanish.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
